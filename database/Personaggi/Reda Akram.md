---
base: "[[database/Personaggi/Personaggi.base]]"
gregorian-date: 1999-04-09
---
#TODO wippone
```dataviewjs
const dt = dv.current()["gregorian-date"];

// ── Normalizzazione al calendario delle Sorelle ──────────────────────────────
const doy    = dt.ordinal;
const y      = dt.year;
const isLeap = y % 4 === 0 && (y % 100 !== 0 || y % 400 === 0);
const adj    = (isLeap && doy > 60) ? doy - 1 : doy;
const fin    = adj > 364 ? 364 : adj;
const fDoy   = (fin - 79 + 364) % 364 + 1;

// ── 1. Data nel Calendario delle Sorelle ─────────────────────────────────────
function getSorelleDate(f) {
  if (f <=  36) return f           + " Primula";
  if (f <=  73) return (f -  36)   + " Rodendron";
  if (f <= 109) return (f -  73)   + " Helianthus";
  if (f <= 146) return (f - 109)   + " Lobelia";
  if (f <= 182) return (f - 146)   + " Tropaleum";
  if (f <= 218) return (f - 182)   + " Aster";
  if (f <= 255) return (f - 218)   + " Mirabilis";
  if (f <= 291) return (f - 255)   + " Ilex";
  if (f <= 328) return (f - 291)   + " Galanthus";
  return          (f - 328)        + " Calycantum";
}

// ── 2. Segno Zodiacale ────────────────────────────────────────────────────────
function getSegno(f) {
  if (f >= 18  && f <= 45 ) return "🦀 Granchio dell'Alba";
  if (f >= 46  && f <= 73 ) return "🦌 Cervo Fiorito";
  if (f >= 74  && f <= 101) return "🦊 Volpe Dorata";
  if (f >= 102 && f <= 129) return "🦅 Aquila dei Venti";
  if (f >= 130 && f <= 157) return "🔥 Salamandra del Focolare";
  if (f >= 158 && f <= 185) return "🐢 Tartaruga delle Maree";
  if (f >= 186 && f <= 213) return "🐲 Drago Cremisi";
  if (f >= 214 && f <= 241) return "🐺 Lupo Lunare";
  if (f >= 242 && f <= 269) return "⛰️ Titano di Roccia";
  if (f >= 270 && f <= 297) return "🐻 Orso delle Bacche";
  if (f >= 298 && f <= 325) return "🦉 Gufo Stellato";
  if (f >= 326 && f <= 353) return "🦄 Unicorno del Gelo";
  return "🐸 Rospo di Giada";
}

// ── 3. Data nel Calendario Fantasy (stagioni + settimana) ─────────────────────
function getFantasyDate(f) {
  const seasons  = ["Blomsol", "Jarnlogi", "Hjartalefi", "Vetrvindur"];
  const weekdays = ["Lunaem", "Martor", "Mecreth", "Jofur", "Vanir", "Saturnia", "Ilios"];
  const si  = Math.floor((f - 1) / 91);
  const dis = (f - 1) % 91 + 1;
  const wk  = Math.ceil(dis / 7);
  const wi  = (f - 1) % 7;
  return wk + "° " + weekdays[wi] + " di " + (seasons[si] || "Vetrvindur");
}

// ── Output ────────────────────────────────────────────────────────────────────
dv.paragraph(`📅 **Data Gregoriana:** ${dt.toFormat("dd/MM/yyyy")}`);
dv.paragraph(`🌸 **Calendario delle Sorelle:** ${getSorelleDate(fDoy)}`);
dv.paragraph(`✨ **Segno Zodiacale:** ${getSegno(fDoy)}`);
dv.paragraph(`🗓️ **Data Fantasy:** ${getFantasyDate(fDoy)}`);
```


![[Reda Akram.jpg]]
