# Quick Launch — PWA pro rychlé spouštění webů

Speed-dial dlaždice s favicony. Klik otevře web. Funguje jako ikona na ploše i offline (shell).

## Soubory
- `index.html` — aplikace
- `manifest.json` — název, ikony, celoobrazovkový režim
- `sw.js` — service worker (offline + auto-aktualizace, network-first)
- `icon-192.png`, `icon-512.png`, `icon-180.png`, `icon-maskable-512.png`

Všechny musí zůstat pohromadě v kořeni repozitáře.

## Nasazení na GitHub Pages
1. Nové **public** repo (např. `quick-launch`).
2. Nahraj **obsah** tohoto zipu (ne zip) do kořene.
3. Settings → Pages → Source **Deploy from a branch**, branch **main**, složka **/ (root)**.
4. Custom domain nech **prázdné**.
5. Adresa: `https://TVOJE-JMENO.github.io/quick-launch/`.

## Ikona na plochu
Otevři adresu v Chrome → ⋮ → **Přidat na plochu**. Poprvé s internetem (uloží se offline shell).

## Používání
- **+ Přidat** — vlož URL (ikona se stáhne z webu sama), volitelně vlastní název a ikonu.
- **hledat…** — filtruje dlaždice.
- **Upravit** — přepne do režimu úprav: klik na dlaždici otevře úpravu, křížek maže.
- **Nastavení** — záloha/obnova do souboru (i s vlastními ikonami).

## Pozn.
- Favicony se tahají z Google favicon služby a potřebují internet; když se nenačtou, ukáže se písmenko.
- Při úpravě appky zvyš ve `sw.js` `quicklaunch-v1` → `-v2`.
