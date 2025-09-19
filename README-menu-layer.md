# 📜 README – menu-layer

Deze layer bevat alle navigatiecomponenten van de website, inclusief hamburgerknop, submenu's en toggling-mechanismen. De CSS is modulair opgebouwd en gekoppeld via `@layer menu` voor cascadecontrole.

---

## 🔗 Bestanden

- `navigation-menu.css` – hoofdstylesheet voor navigatie
- `CHANGELOG-menu-layer.md` – forensic logboek van wijzigingen
- `README-menu-layer.md` – deze uitleg

---

## 🧠 Cascade-impact

- Beïnvloedt alleen `.nav-openZ`, `.submenu`, `.dropdown`
- Geen impact op `theme-layer`, `layout-layer`, of externe stylesheets
- Gekoppeld via `@layer menu` in de globale CSS-opbouw

---

## 🧪 Teststrategie

- Getest in Phoenix Code met `testpage.html`
- DevTools gebruikt voor cascade-verificatie
- Mobile UX getest via touch-simulatie
- Rollbacks vastgelegd in changelog per versie

---

## ✅ Stabiele versies

- `v1.0-navigatie-werkend` – basisstructuur, cascade correct
- `v1.1-hover-fix` – verbeterde submenu-hover, mobile getest

Zie `CHANGELOG-menu-layer.md` voor volledige versiegeschiedenis en rollback-verwijzingen.
