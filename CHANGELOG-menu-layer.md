# 📜 Changelog – menu-layer

Dit logboek documenteert alle wijzigingen aan de navigatiecomponenten binnen de `@layer menu`. Elke entry is traceerbaar, modulair en afgestemd op de cascade-impact.

---

## ✅ Stabiele versies

- `v1.0-navigatie-werkend` – basisstructuur werkend, `.nav-openZ` cascade functioneert correct
- `v1.1-hover-fix` – submenu-hover verbeterd, mobile UX getest

---

## 📅 Wijzigingen per datum

### [2025-09-18]
- `.nav-openZ` cascade gefixed voor submenu
- Hover-stijl submenu verbeterd voor mobile UX
- Handmatige activatie getest via DevTools

### [2025-09-19]
- JS-trigger toegevoegd voor toggling `.nav-openZ`
- Cascade getest in Blogger-template
- DevTools snapshot gemaakt van cascade vóór/na

---

## 🧠 Notities

- Alle wijzigingen zijn getest in `menu-layer` branch vóór merge naar `main`
- CSS-layer `@layer menu` is actief en correct gekoppeld aan `navigation-menu.css`
- Geen impact op andere layers zoals `theme`, `layout` of `blogger-css`

---



