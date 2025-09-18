# 🔧 Configuratiebeheer voor CSS-layers en Git-branches

Deze repository gebruikt een modulair configuratiebeheer waarbij elke CSS-layer correspondeert met een Git-branch. Zo kunnen wijzigingen per cascade-laag worden getest, gevalideerd en teruggerold zonder impact op andere componenten.

## 🌿 Branchstructuur

| Branchnaam       | Doelgebied in CSS         | CSS-layer            |
|------------------|---------------------------|----------------------|
| `reset-layer`    | Browser resets            | `@layer reset`       |
| `variables-layer`| Design tokens             | `@layer variables`   |
| `base-layer`     | Basis HTML-opmaak         | `@layer base`        |
| `utilities-layer`| Helper-classes            | `@layer utilities`   |
| `theme-layer`    | Visuele stijl & branding  | `@layer theme`       |
| `blogger-layer`  | Blogger-specifieke fixes  | `@layer blogger-css` |
| `layout-layer`   | Containers & positionering| `@layer layout`      |
| `menu-layer`     | Navigatie & dropdowns     | `@layer menu`        |
| `temp-layer`     | Tijdelijke experimenten   | `@layer temp`        |

## 🧠 Commit-conventies

Gebruik commit messages in het volgende formaat:

[layer]: [component] – [actie]


**Voorbeelden:**

- `menu-layer: .nav-openZ – display cascade gefixed voor submenu`
- `theme-layer: buttons – kleurcontrast verbeterd voor accessibility`
- `layout-layer: .container – max-width aangepast voor mobile`

---

## 🧪 Werkwijze

1. Maak een nieuwe branch vanuit `main`
2. Werk alleen aan het bijbehorende CSS-bestand of layer
3. Commit met duidelijke message
4. Open een Pull Request → controleer visueel wat er verandert
5. Merge pas als het stabiel is

---

## 🏷️ Tags en releases

Gebruik tags om stabiele versies vast te leggen:

- `v1.0-navigatie-werkend`
- `v1.1-hover-fix`
- `v2.0-mobile-ready`

Ga naar tab “Releases” in GitHub → “Draft a new release” → voeg changelog toe

---

## 📦 Bestandstructuur (aanbevolen)

/css/ 
├── reset.css 
├── variables.css 
├── base.css 
├── utilities.css 
├── theme.css 
├── blogger.css 
├── layout.css 
├── navigation-menu.css 
└── temp.css


Combineer via `<link>` in HTML of bundel via build-tool.

---

## 📚 Changelog-template per layer

Je kunt per branch een changelog bijhouden in een apart bestand:

**Voorbeeld: `CHANGELOG-menu-layer.md`**

menu-layer changelog
- [2025-09-18] .nav-openZ cascade gefixed voor submenu
- [2025-09-19] hover-stijl verbeterd voor mobile UX


Zo hou je per layer een logboek bij — future-proof en rollbackbaar.

---

