# Z-Index Stacking Order — Chi tiết Selectors

> Sắp xếp từ **CAO → THẤP**. Mỗi selector ghi rõ file, dòng, và ngữ cảnh sử dụng.

---

## 🔴 z: 10000 — `$base-z-index-overlay-fullscreen`

| # | Selector | Ngữ cảnh | File |
|---|---|---|---|
| 1 | `.search-results-tabs-container` | Mobile fullscreen filter panel (`position: fixed; inset: 0`) — chỉ active trên `breakpoint-down(md)` | [_search-results.scss:112](file:///Users/tri.nguyen/Project/aemaacs-investments-BE/aemaacs-investments/mandg-investments/ui.frontend/src/main/webpack/scss/base/6-components/search-results/_search-results.scss#L112) |

---

## 🔴 z: 9999 — `$base-z-index-ui-skip-to-main-link`

| # | Selector | Ngữ cảnh | File |
|---|---|---|---|
| 1 | `.header-top` | Top header bar (chứa language selector, audience links) — `position: relative` | [_top-header.scss:15](file:///Users/tri.nguyen/Project/aemaacs-investments-BE/aemaacs-investments/mandg-investments/ui.frontend/src/main/webpack/scss/base/6-components/mega-menu/top-header/_top-header.scss#L15) |
| 2 | `.header-menu-button` | Nút CTA trong menu mobile (nằm `position: absolute; bottom: 0` trong menu panel) | [_header-menu.scss:61](file:///Users/tri.nguyen/Project/aemaacs-investments-BE/aemaacs-investments/mandg-investments/ui.frontend/src/main/webpack/scss/base/6-components/mega-menu/_header-menu.scss#L61) |
| 3 | `.filter__form-toggle-button[aria-expanded='true']` | Nút toggle filter trên mobile khi mở — `position: fixed; top: 0` | [_filter-form-item.scss:384](file:///Users/tri.nguyen/Project/aemaacs-investments-BE/aemaacs-investments/mandg-investments/ui.frontend/src/main/webpack/scss/base/7-utilities/filter-form-item/_filter-form-item.scss#L384) |

---

## 🟠 z: 1000 — `$base-z-index-overlay-modal` + `$base-z-index-ui-back-to-top`

> [!WARNING]
> **Hai token khác nhau, CÙNG giá trị 1000** — có thể gây chồng chéo giữa modal và banner.

### Token: `overlay-modal` (1000)

| # | Selector | Ngữ cảnh | File |
|---|---|---|---|
| 1 | `.popup`, `.popup-static` | Popup/modal wrapper — `position: fixed; inset: 0` | [_popup.scss:132](file:///Users/tri.nguyen/Project/aemaacs-investments-BE/aemaacs-investments/mandg-investments/ui.frontend/src/main/webpack/scss/base/3-generics/_popup.scss#L132) |
| 2 | `.main-menu-dropdown` | Mega menu dropdown panel — `position: absolute` | [_nav-item.scss:11](file:///Users/tri.nguyen/Project/aemaacs-investments-BE/aemaacs-investments/mandg-investments/ui.frontend/src/main/webpack/scss/base/6-components/mega-menu/nav-item/_nav-item.scss#L11) |
| 3 | `.attestation-close-button` | Nút đóng attestation — `position: absolute; top/right: -20px` | [_attestation.scss:128](file:///Users/tri.nguyen/Project/aemaacs-investments-BE/aemaacs-investments/mandg-investments/ui.frontend/src/main/webpack/scss/base/6-components/attestation/_attestation.scss#L128) |
| 4 | `.attestation-dropdown-wrapper` | Attestation dropdown — `position: absolute; top: calc(100% + spacing)` | [_attestation.scss:405](file:///Users/tri.nguyen/Project/aemaacs-investments-BE/aemaacs-investments/mandg-investments/ui.frontend/src/main/webpack/scss/base/6-components/attestation/_attestation.scss#L405) |

### Token: `ui-back-to-top` (1000)

| # | Selector | Ngữ cảnh | File |
|---|---|---|---|
| 5 | `.header-fixed` | Toàn bộ header — `position: fixed; top/left/right: 0` | [_header-base.scss:33](file:///Users/tri.nguyen/Project/aemaacs-investments-BE/aemaacs-investments/mandg-investments/ui.frontend/src/main/webpack/scss/base/6-components/mega-menu/_header-base.scss#L33) |
| 6 | `.text-error-message` (inside `.experiencefragment` or `:has(~ .header-fixed)`) | Error message banner — `position: absolute; top: 0; width: 100%` | [_text-error-message.scss:15](file:///Users/tri.nguyen/Project/aemaacs-investments-BE/aemaacs-investments/mandg-investments/ui.frontend/src/main/webpack/scss/base/6-components/text/_text-error-message.scss#L15) |
| 7 | `.dismissible-service-banner-v2:has(~ .header-fixed)` | Dismissible banner — `position: fixed; top: 0; width: 100%` | [_dismissible-service-banner.scss:33](file:///Users/tri.nguyen/Project/aemaacs-investments-BE/aemaacs-investments/mandg-investments/ui.frontend/src/main/webpack/scss/base/6-components/dismissible-service-banner/_dismissible-service-banner.scss#L33) |
| 8 | `.filter__form` (mobile) | Filter form overlay — `position: fixed; inset: 0` trên `breakpoint-down(lg)` | [_filter-form-item.scss:502](file:///Users/tri.nguyen/Project/aemaacs-investments-BE/aemaacs-investments/mandg-investments/ui.frontend/src/main/webpack/scss/base/7-utilities/filter-form-item/_filter-form-item.scss#L502) |

---

## 🟡 z: 900 — `$base-z-index-ui-popover`

| # | Selector | Ngữ cảnh | File |
|---|---|---|---|
| 1 | `.fund-charge-calc .toggle-section` | Calculator toggle section — mở/đóng nội dung tính toán | [_toggle-section.scss:9](file:///Users/tri.nguyen/Project/aemaacs-investments-BE/aemaacs-investments/mandg-investments/ui.frontend/src/main/webpack/scss/base/6-components/fund-charge-calculator/components/_toggle-section.scss#L9) |

---

## 🟡 z: 700 — `$base-z-index-ui-navigation`

| # | Selector | Ngữ cảnh | File |
|---|---|---|---|
| 1 | `.header-menu` (mobile) | Menu navigation panel — `position: fixed; inset` — chỉ trên `breakpoint-down(md)` | [_header-menu.scss:20](file:///Users/tri.nguyen/Project/aemaacs-investments-BE/aemaacs-investments/mandg-investments/ui.frontend/src/main/webpack/scss/base/6-components/mega-menu/_header-menu.scss#L20) |

---

## 🟢 z: 600 — `$base-z-index-ui-header`

| # | Selector | Ngữ cảnh | File |
|---|---|---|---|
| 1 | `.marketing-label` | Marketing communication label — `position: fixed; right: 0` (rotated label ở cạnh phải page) | [_marketing-communication.scss:22](file:///Users/tri.nguyen/Project/aemaacs-investments-BE/aemaacs-investments/mandg-investments/ui.frontend/src/main/webpack/scss/base/6-components/marketing-communication/_marketing-communication.scss#L22) |

---

## 🟢 z: 500 — `$base-z-index-ui-sidebar`

| # | Selector | Ngữ cảnh | File |
|---|---|---|---|
| 1 | `.article-header` (desktop sidebar) | Article header sidebar layout — nội dung bên phải | [_article-header.scss:120](file:///Users/tri.nguyen/Project/aemaacs-investments-BE/aemaacs-investments/mandg-investments/ui.frontend/src/main/webpack/scss/base/6-components/article-header/_article-header.scss#L120) |
| 2 | `.article-header` (desktop sidebar variant 2) | Variant khác của sidebar layout | [_article-header.scss:225](file:///Users/tri.nguyen/Project/aemaacs-investments-BE/aemaacs-investments/mandg-investments/ui.frontend/src/main/webpack/scss/base/6-components/article-header/_article-header.scss#L225) |
| 3 | `.fund-charge-calc .field` (focus state) | Calculator input field khi có focus — đẩy lên trên các field khác | [_field.scss:96](file:///Users/tri.nguyen/Project/aemaacs-investments-BE/aemaacs-investments/mandg-investments/ui.frontend/src/main/webpack/scss/base/6-components/fund-charge-calculator/components/_field.scss#L96) |

---

## 🔵 z: 400 — `$base-z-index-ui-overlay-backdrop`

| # | Selector | Ngữ cảnh | File |
|---|---|---|---|
| 1 | `.cmp-breadcrumb` | Breadcrumb — `position: absolute; top: ...` — nằm đè trên hero banner | [_breadcrumb.scss:12](file:///Users/tri.nguyen/Project/aemaacs-investments-BE/aemaacs-investments/mandg-investments/ui.frontend/src/main/webpack/scss/base/6-components/breadcrumb/_breadcrumb.scss#L12) |
| 2 | `.navigation--type-fund-page` | Fund page tab navigation — `position: sticky; top: header-height` | [_navigation-fund-page.scss:13](file:///Users/tri.nguyen/Project/aemaacs-investments-BE/aemaacs-investments/mandg-investments/ui.frontend/src/main/webpack/scss/base/6-components/navigation/_navigation-fund-page.scss#L13) |
| 3 | `.fund-charge-calc .toggle-section` (backdrop) | Calculator toggle backdrop overlay | [_toggle-section.scss:89](file:///Users/tri.nguyen/Project/aemaacs-investments-BE/aemaacs-investments/mandg-investments/ui.frontend/src/main/webpack/scss/base/6-components/fund-charge-calculator/components/_toggle-section.scss#L89) |

---

## 🔵 z: 300 — `$base-z-index-ui-fixed`

| # | Selector | Ngữ cảnh | File |
|---|---|---|---|
| 1 | `.social-share__inner` (desktop) | Social share icons — `position: absolute; top: 100%` — chỉ trên `breakpoint-up(md)` | [_social-share.scss:59](file:///Users/tri.nguyen/Project/aemaacs-investments-BE/aemaacs-investments/mandg-investments/ui.frontend/src/main/webpack/scss/base/6-components/social-share/_social-share.scss#L59) |

---

## 🔵 z: 200 — `$base-z-index-ui-sticky`

| # | Selector | Ngữ cảnh | File |
|---|---|---|---|
| 1 | `.cmp-experiencefragment .container--sticky` | Container sticky — `position: fixed; top: 0; left: 0; right: 0` | [_container-pin-top.scss:12](file:///Users/tri.nguyen/Project/aemaacs-investments-BE/aemaacs-investments/mandg-investments/ui.frontend/src/main/webpack/scss/base/6-components/container/_container-pin-top.scss#L12) |
| 2 | `.in-page-navigation-top` (sticky state) | In-page nav top — sticky khi scroll | [_in-page-navigation-top.scss:135](file:///Users/tri.nguyen/Project/aemaacs-investments-BE/aemaacs-investments/mandg-investments/ui.frontend/src/main/webpack/scss/base/6-components/in-page-navigation/_in-page-navigation-top.scss#L135) |
| 3 | `.printbutton:has(.print-button-cmp__inner--float-*)` | Print button — `position: sticky; bottom: 0` | [_print-button.scss:57](file:///Users/tri.nguyen/Project/aemaacs-investments-BE/aemaacs-investments/mandg-investments/ui.frontend/src/main/webpack/scss/base/6-components/print-button/_print-button.scss#L57) |
| 4 | `.article-header` (sticky bar) | Article header khi sticky | [_article-header.scss:258](file:///Users/tri.nguyen/Project/aemaacs-investments-BE/aemaacs-investments/mandg-investments/ui.frontend/src/main/webpack/scss/base/6-components/article-header/_article-header.scss#L258) |

---

## ⚪ z: 100 — `$base-z-index-ui-dropdown`

| # | Selector | Ngữ cảnh | File |
|---|---|---|---|
| 1 | `.search-category-filter-list` | Filter dropdown list — `position: absolute; top: 100%` | [_filter-form-item.scss:249](file:///Users/tri.nguyen/Project/aemaacs-investments-BE/aemaacs-investments/mandg-investments/ui.frontend/src/main/webpack/scss/base/7-utilities/filter-form-item/_filter-form-item.scss#L249) |
| 2 | `.searchbox__dropdown` | Search box autocomplete dropdown — `position: absolute` | [_search-box.scss:232](file:///Users/tri.nguyen/Project/aemaacs-investments-BE/aemaacs-investments/mandg-investments/ui.frontend/src/main/webpack/scss/base/6-components/search-box/_search-box.scss#L232) |
| 3 | `.social-share__items--pinned` | Social share pinned variant — `position: sticky` | [_social-share.scss:81](file:///Users/tri.nguyen/Project/aemaacs-investments-BE/aemaacs-investments/mandg-investments/ui.frontend/src/main/webpack/scss/base/6-components/social-share/_social-share.scss#L81) |
| 4 | `.header-audience .header-attestation` | Header attestation modal — `position: fixed; inset: 0` | [_header-audience.scss:16](file:///Users/tri.nguyen/Project/aemaacs-investments-BE/aemaacs-investments/mandg-investments/ui.frontend/src/main/webpack/scss/base/6-components/mega-menu/_header-audience.scss#L16) |
| 5 | `.header-dropdown__list` (top-header) | Top header dropdown list | [_top-header-dropdown.scss:94](file:///Users/tri.nguyen/Project/aemaacs-investments-BE/aemaacs-investments/mandg-investments/ui.frontend/src/main/webpack/scss/base/6-components/mega-menu/top-header/_top-header-dropdown.scss#L94) |
| 6 | `.fund-charge-calc .toggle-section` (dropdown) | Calculator toggle dropdown content | [_toggle-section.scss:119](file:///Users/tri.nguyen/Project/aemaacs-investments-BE/aemaacs-investments/mandg-investments/ui.frontend/src/main/webpack/scss/base/6-components/fund-charge-calculator/components/_toggle-section.scss#L119) |

---

## ⚪ z: 10 — `$base-z-index-content-elevated`

| # | Selector | Ngữ cảnh | File |
|---|---|---|---|
| 1 | `.popup-inner` | Popup inner content — `position: relative` | [_popup.scss:93](file:///Users/tri.nguyen/Project/aemaacs-investments-BE/aemaacs-investments/mandg-investments/ui.frontend/src/main/webpack/scss/base/3-generics/_popup.scss#L93) |
| 2 | `table th` (sticky header) | Table base sticky header cell | [_table-base.scss:26](file:///Users/tri.nguyen/Project/aemaacs-investments-BE/aemaacs-investments/mandg-investments/ui.frontend/src/main/webpack/scss/base/6-components/table/_table-base.scss#L26) |
| 3 | `table thead` (sticky) | Table base sticky thead | [_table-base.scss:50](file:///Users/tri.nguyen/Project/aemaacs-investments-BE/aemaacs-investments/mandg-investments/ui.frontend/src/main/webpack/scss/base/6-components/table/_table-base.scss#L50) |
| 4 | `.advance-sorting-column` (tooltip) | Advance table sorting tooltip | [_advance-sorting-column.scss:110](file:///Users/tri.nguyen/Project/aemaacs-investments-BE/aemaacs-investments/mandg-investments/ui.frontend/src/main/webpack/scss/base/6-components/table/advance-table/_advance-sorting-column.scss#L110) |
| 5 | `.in-page-navigation-top-wrapper` | In-page navigation bar elevated | [_in-page-navigation-top.scss:263](file:///Users/tri.nguyen/Project/aemaacs-investments-BE/aemaacs-investments/mandg-investments/ui.frontend/src/main/webpack/scss/base/6-components/in-page-navigation/_in-page-navigation-top.scss#L263) |
| 6 | `.container` (elevated) | Container elevated variant | [_container.scss:48](file:///Users/tri.nguyen/Project/aemaacs-investments-BE/aemaacs-investments/mandg-investments/ui.frontend/src/main/webpack/scss/base/6-components/container/_container.scss#L48) |
| 7 | `.fund-charge-calc .field` (elevated) | Calculator field elevated state | [_field.scss:26](file:///Users/tri.nguyen/Project/aemaacs-investments-BE/aemaacs-investments/mandg-investments/ui.frontend/src/main/webpack/scss/base/6-components/fund-charge-calculator/components/_field.scss#L26) |
| 8 | `.fund-charge-calc .toggle-section` (content) | Calculator toggle section inner content | [_toggle-section.scss:141](file:///Users/tri.nguyen/Project/aemaacs-investments-BE/aemaacs-investments/mandg-investments/ui.frontend/src/main/webpack/scss/base/6-components/fund-charge-calculator/components/_toggle-section.scss#L141) |
| 9 | `.related-content` (elevated card) | Related content card elevated | [_related-content.scss:278](file:///Users/tri.nguyen/Project/aemaacs-investments-BE/aemaacs-investments/mandg-investments/ui.frontend/src/main/webpack/scss/base/6-components/related-content/_related-content.scss#L278) |

---

## ⚪ z: 3 — `$base-z-index-content-level-3`

| # | Selector | Ngữ cảnh | File |
|---|---|---|---|
| 1 | `.popup-is-close` | Popup close button — `position: absolute; top/right` | [_popup.scss:151](file:///Users/tri.nguyen/Project/aemaacs-investments-BE/aemaacs-investments/mandg-investments/ui.frontend/src/main/webpack/scss/base/3-generics/_popup.scss#L151) |
| 2 | `.swiper-wrapper` | Swiper main wrapper | [_swiper.scss:17](file:///Users/tri.nguyen/Project/aemaacs-investments-BE/aemaacs-investments/mandg-investments/ui.frontend/src/main/webpack/scss/base/3-generics/swiper/_swiper.scss#L17) |
| 3 | `.content-tile-with-video__wrapper` | Content tile video wrapper | [_content-tile-with-video.scss:15](file:///Users/tri.nguyen/Project/aemaacs-investments-BE/aemaacs-investments/mandg-investments/ui.frontend/src/main/webpack/scss/base/6-components/content-tile/_content-tile-with-video.scss#L15) |
| 4 | `.advance-table thead th` (fixed header) | Advance table fixed first row header cell | [_advance-fixed-first-row-column.scss:42](file:///Users/tri.nguyen/Project/aemaacs-investments-BE/aemaacs-investments/mandg-investments/ui.frontend/src/main/webpack/scss/base/6-components/table/advance-table/_advance-fixed-first-row-column.scss#L42) |
| 5 | `.advance-table .scroll-bar` | Advance table custom scroll bar | [_advance-scroll-bar.scss:34](file:///Users/tri.nguyen/Project/aemaacs-investments-BE/aemaacs-investments/mandg-investments/ui.frontend/src/main/webpack/scss/base/6-components/table/advance-table/_advance-scroll-bar.scss#L34) |
| 6 | `.advance-sorting-column` (sorting icon) | Advance table sorting icon column | [_advance-sorting-column.scss:70](file:///Users/tri.nguyen/Project/aemaacs-investments-BE/aemaacs-investments/mandg-investments/ui.frontend/src/main/webpack/scss/base/6-components/table/advance-table/_advance-sorting-column.scss#L70) |
| 7 | `.slider__nav` | Slider navigation arrows | [_slider.scss:27](file:///Users/tri.nguyen/Project/aemaacs-investments-BE/aemaacs-investments/mandg-investments/ui.frontend/src/main/webpack/scss/base/6-components/slider/_slider.scss#L27) |
| 8 | `.related-content__card-overlay` | Related content card overlay | [_related-content.scss:259](file:///Users/tri.nguyen/Project/aemaacs-investments-BE/aemaacs-investments/mandg-investments/ui.frontend/src/main/webpack/scss/base/6-components/related-content/_related-content.scss#L259) |
| 9 | `.in-page-navigation__active-indicator` | In-page navigation active tab indicator | [_in-page-navigation.scss:71](file:///Users/tri.nguyen/Project/aemaacs-investments-BE/aemaacs-investments/mandg-investments/ui.frontend/src/main/webpack/scss/base/6-components/in-page-navigation/_in-page-navigation.scss#L71) |

---

## ⚪ z: 2 — `$base-z-index-content-level-2`

| # | Selector | Ngữ cảnh | File |
|---|---|---|---|
| 1 | `.popup-content` | Popup content wrapper | [_popup.scss:72](file:///Users/tri.nguyen/Project/aemaacs-investments-BE/aemaacs-investments/mandg-investments/ui.frontend/src/main/webpack/scss/base/3-generics/_popup.scss#L72) |
| 2 | `.content-tile__overlay` | Content tile hover overlay | [_content-tile.scss:55](file:///Users/tri.nguyen/Project/aemaacs-investments-BE/aemaacs-investments/mandg-investments/ui.frontend/src/main/webpack/scss/base/6-components/content-tile/_content-tile.scss#L55) |
| 3 | `.table-base thead th` (scroll shadow) | Table base scroll shadow | [_table-base.scss:85](file:///Users/tri.nguyen/Project/aemaacs-investments-BE/aemaacs-investments/mandg-investments/ui.frontend/src/main/webpack/scss/base/6-components/table/_table-base.scss#L85) |
| 4 | `.table-fixed-first-column td:first-child` | Table fixed first column | [_table-fixed-first-column.scss:11](file:///Users/tri.nguyen/Project/aemaacs-investments-BE/aemaacs-investments/mandg-investments/ui.frontend/src/main/webpack/scss/base/6-components/table/_table-fixed-first-column.scss#L11) |
| 5 | `.advance-table tbody td:first-child` (fixed) | Advance table fixed first column body | [_advance-fixed-first-row-column.scss:21](file:///Users/tri.nguyen/Project/aemaacs-investments-BE/aemaacs-investments/mandg-investments/ui.frontend/src/main/webpack/scss/base/6-components/table/advance-table/_advance-fixed-first-row-column.scss#L21) |
| 6 | `.glossary-filters__letter::before` | Glossary filter letter before pseudo | [_glossary-filters.scss:109](file:///Users/tri.nguyen/Project/aemaacs-investments-BE/aemaacs-investments/mandg-investments/ui.frontend/src/main/webpack/scss/base/6-components/glossary/_glossary-filters.scss#L109) |
| 7 | `.glossary-filters__letter::after` | Glossary filter letter after pseudo | [_glossary-filters.scss:115](file:///Users/tri.nguyen/Project/aemaacs-investments-BE/aemaacs-investments/mandg-investments/ui.frontend/src/main/webpack/scss/base/6-components/glossary/_glossary-filters.scss#L115) |
| 8 | `.hero-banner-with-tiles` (5 lần) | Hero banner tiles content/overlays — nhiều variant | [_hero-banner-with-tiles.scss:90,180,315,333,380](file:///Users/tri.nguyen/Project/aemaacs-investments-BE/aemaacs-investments/mandg-investments/ui.frontend/src/main/webpack/scss/base/6-components/hero-banner-with-tiles/_hero-banner-with-tiles.scss#L90) |
| 9 | `.icon-tile__hover` | Icon tile hover state overlay | [_icon-tile.scss:88](file:///Users/tri.nguyen/Project/aemaacs-investments-BE/aemaacs-investments/mandg-investments/ui.frontend/src/main/webpack/scss/base/6-components/icon-tile/_icon-tile.scss#L88) |
| 10 | `.container__section` | Container section layout | [_container.scss:230](file:///Users/tri.nguyen/Project/aemaacs-investments-BE/aemaacs-investments/mandg-investments/ui.frontend/src/main/webpack/scss/base/6-components/container/_container.scss#L230) |
| 11 | `.slider-images__item` | Slider images item | [_slider-images.scss:25](file:///Users/tri.nguyen/Project/aemaacs-investments-BE/aemaacs-investments/mandg-investments/ui.frontend/src/main/webpack/scss/base/6-components/slider/_slider-images.scss#L25) |
| 12 | `.search-results-items__card` | Search results card item | [_search-results-items.scss:122](file:///Users/tri.nguyen/Project/aemaacs-investments-BE/aemaacs-investments/mandg-investments/ui.frontend/src/main/webpack/scss/base/6-components/search-results/_search-results-items.scss#L122) |
| 13 | `.related-content__section` | Related content section | [_related-content.scss:357](file:///Users/tri.nguyen/Project/aemaacs-investments-BE/aemaacs-investments/mandg-investments/ui.frontend/src/main/webpack/scss/base/6-components/related-content/_related-content.scss#L357) |
| 14 | `.navigation__arrow` | Fund page navigation arrows | [_navigation-fund-page.scss:97](file:///Users/tri.nguyen/Project/aemaacs-investments-BE/aemaacs-investments/mandg-investments/ui.frontend/src/main/webpack/scss/base/6-components/navigation/_navigation-fund-page.scss#L97) |
| 15 | `.navigation__arrow span` | Arrow span inside | [_navigation-fund-page.scss:104](file:///Users/tri.nguyen/Project/aemaacs-investments-BE/aemaacs-investments/mandg-investments/ui.frontend/src/main/webpack/scss/base/6-components/navigation/_navigation-fund-page.scss#L104) |
| 16 | `.fund-charge-calc .results-table th` | Calculator results table header | [_results-table.scss:24](file:///Users/tri.nguyen/Project/aemaacs-investments-BE/aemaacs-investments/mandg-investments/ui.frontend/src/main/webpack/scss/base/6-components/fund-charge-calculator/components/_results-table.scss#L24) |
| 17 | `.fund-charge-calc .dropdown__wrapper` | Calculator dropdown wrapper | [_dropdown.scss:12](file:///Users/tri.nguyen/Project/aemaacs-investments-BE/aemaacs-investments/mandg-investments/ui.frontend/src/main/webpack/scss/base/6-components/fund-charge-calculator/components/_dropdown.scss#L12) |
| 18 | `.fund-charge-calc .input` (variants) | Calculator input field variants | [_input.scss:83,98](file:///Users/tri.nguyen/Project/aemaacs-investments-BE/aemaacs-investments/mandg-investments/ui.frontend/src/main/webpack/scss/base/6-components/fund-charge-calculator/components/_input.scss#L83) |

---

## ⚪ z: 1 — `$base-z-index-content-level-1`

| # | Selector | Ngữ cảnh | File |
|---|---|---|---|
| 1 | `.popup-container` | Popup container — `position: absolute; inset: 0` | [_popup.scss:38](file:///Users/tri.nguyen/Project/aemaacs-investments-BE/aemaacs-investments/mandg-investments/ui.frontend/src/main/webpack/scss/base/3-generics/_popup.scss#L38) |
| 2 | `.button` (mixin) | Button base content — `position: relative` | [_button.mixins.scss:19](file:///Users/tri.nguyen/Project/aemaacs-investments-BE/aemaacs-investments/mandg-investments/ui.frontend/src/main/webpack/scss/base/6-components/button/_button.mixins.scss#L19) |
| 3 | `.promotional-banner__content` | Promotional banner content text | [_promotional-banner.scss:88](file:///Users/tri.nguyen/Project/aemaacs-investments-BE/aemaacs-investments/mandg-investments/ui.frontend/src/main/webpack/scss/base/6-components/promotional-banner/_promotional-banner.scss#L88) |
| 4 | `.search-box__input` | Search box input field | [_search-box.scss:90](file:///Users/tri.nguyen/Project/aemaacs-investments-BE/aemaacs-investments/mandg-investments/ui.frontend/src/main/webpack/scss/base/6-components/search-box/_search-box.scss#L90) |
| 5 | `.text-error-message__close` | Error message close button | [_text-error-message.scss:34](file:///Users/tri.nguyen/Project/aemaacs-investments-BE/aemaacs-investments/mandg-investments/ui.frontend/src/main/webpack/scss/base/6-components/text/_text-error-message.scss#L34) |
| 6 | `.content-tile-with-video__play-btn` | Video tile play button | [_content-tile-with-video.scss:50](file:///Users/tri.nguyen/Project/aemaacs-investments-BE/aemaacs-investments/mandg-investments/ui.frontend/src/main/webpack/scss/base/6-components/content-tile/_content-tile-with-video.scss#L50) |
| 7 | `.icon-tile__content` | Icon tile content layer | [_icon-tile.scss:41](file:///Users/tri.nguyen/Project/aemaacs-investments-BE/aemaacs-investments/mandg-investments/ui.frontend/src/main/webpack/scss/base/6-components/icon-tile/_icon-tile.scss#L41) |
| 8 | `.icon-tile__icon` | Icon tile icon layer | [_icon-tile.scss:50](file:///Users/tri.nguyen/Project/aemaacs-investments-BE/aemaacs-investments/mandg-investments/ui.frontend/src/main/webpack/scss/base/6-components/icon-tile/_icon-tile.scss#L50) |
| 9 | `.container--sticky` inner banners | Container sticky inner banners (dismissible, error, compliance) | [_container-pin-top.scss:17](file:///Users/tri.nguyen/Project/aemaacs-investments-BE/aemaacs-investments/mandg-investments/ui.frontend/src/main/webpack/scss/base/6-components/container/_container-pin-top.scss#L17) |
| 10 | `.container__content` | Container content | [_container.scss:320](file:///Users/tri.nguyen/Project/aemaacs-investments-BE/aemaacs-investments/mandg-investments/ui.frontend/src/main/webpack/scss/base/6-components/container/_container.scss#L320) |
| 11 | `.hero-banner__content` | Hero banner content overlay | [_hero-banner.scss:266](file:///Users/tri.nguyen/Project/aemaacs-investments-BE/aemaacs-investments/mandg-investments/ui.frontend/src/main/webpack/scss/base/6-components/hero-banner/_hero-banner.scss#L266) |
| 12 | `.hero-banner-video__content` | Hero banner video content | [_hero-banner-video.scss:12](file:///Users/tri.nguyen/Project/aemaacs-investments-BE/aemaacs-investments/mandg-investments/ui.frontend/src/main/webpack/scss/base/6-components/hero-banner/_hero-banner-video.scss#L12) |
| 13 | `.hero-banner-center-icon__content` | Hero banner center icon content | [_hero-banner-center-icon-banner.scss:33](file:///Users/tri.nguyen/Project/aemaacs-investments-BE/aemaacs-investments/mandg-investments/ui.frontend/src/main/webpack/scss/base/6-components/hero-banner/_hero-banner-center-icon-banner.scss#L33) |
| 14 | `.slider-ampersand__content` | Slider ampersand content | [_slider-ampersand.scss:149](file:///Users/tri.nguyen/Project/aemaacs-investments-BE/aemaacs-investments/mandg-investments/ui.frontend/src/main/webpack/scss/base/6-components/slider/_slider-ampersand.scss#L149) |
| 15 | `.slider-theme-style__content` | Slider theme style content | [_slider-theme-style.scss:66](file:///Users/tri.nguyen/Project/aemaacs-investments-BE/aemaacs-investments/mandg-investments/ui.frontend/src/main/webpack/scss/base/6-components/slider/_slider-theme-style.scss#L66) |
| 16 | `.top-header-dropdown__inner` | Top header dropdown inner content | [_top-header-dropdown.scss:17](file:///Users/tri.nguyen/Project/aemaacs-investments-BE/aemaacs-investments/mandg-investments/ui.frontend/src/main/webpack/scss/base/6-components/mega-menu/top-header/_top-header-dropdown.scss#L17) |
| 17 | `.top-header-dropdown__link` | Top header dropdown link items | [_top-header-dropdown.scss:126](file:///Users/tri.nguyen/Project/aemaacs-investments-BE/aemaacs-investments/mandg-investments/ui.frontend/src/main/webpack/scss/base/6-components/mega-menu/top-header/_top-header-dropdown.scss#L126) |
| 18 | `.in-page-navigation-left__indicator` | In-page left nav active indicator | [_in-page-navigation-left.scss:279,352](file:///Users/tri.nguyen/Project/aemaacs-investments-BE/aemaacs-investments/mandg-investments/ui.frontend/src/main/webpack/scss/base/6-components/in-page-navigation/_in-page-navigation-left.scss#L279) |
| 19 | `.related-content-ampersands__content` | Related content ampersands content | [_related-content-ampersands.scss:88](file:///Users/tri.nguyen/Project/aemaacs-investments-BE/aemaacs-investments/mandg-investments/ui.frontend/src/main/webpack/scss/base/6-components/related-content/_related-content-ampersands.scss#L88) |
| 20 | `.related-content-ampersands-feature` (3 lần) | Ampersands feature content | [_related-content-ampersands-feature.scss:210,232,333](file:///Users/tri.nguyen/Project/aemaacs-investments-BE/aemaacs-investments/mandg-investments/ui.frontend/src/main/webpack/scss/base/6-components/related-content/_related-content-ampersands-feature.scss#L210) |
| 21 | `.related-content-ampersands-listing__content` | Ampersands listing content | [_related-content-ampersands-listing.scss:49](file:///Users/tri.nguyen/Project/aemaacs-investments-BE/aemaacs-investments/mandg-investments/ui.frontend/src/main/webpack/scss/base/6-components/related-content/_related-content-ampersands-listing.scss#L49) |
| 22 | `.fund-charge-calc .input__label` | Calculator input label | [_input.scss:54](file:///Users/tri.nguyen/Project/aemaacs-investments-BE/aemaacs-investments/mandg-investments/ui.frontend/src/main/webpack/scss/base/6-components/fund-charge-calculator/components/_input.scss#L54) |
| 23 | `.fund-charge-calc .dropdown__label` | Calculator dropdown label | [_dropdown.scss:29](file:///Users/tri.nguyen/Project/aemaacs-investments-BE/aemaacs-investments/mandg-investments/ui.frontend/src/main/webpack/scss/base/6-components/fund-charge-calculator/components/_dropdown.scss#L29) |
| 24 | `.fund-charge-calc .steps__label` | Calculator steps label | [_steps.scss:53](file:///Users/tri.nguyen/Project/aemaacs-investments-BE/aemaacs-investments/mandg-investments/ui.frontend/src/main/webpack/scss/base/6-components/fund-charge-calculator/components/_steps.scss#L53) |

---

## ⚫ z: 0 — `$base-z-index-base-base`

| # | Selector | Ngữ cảnh | File |
|---|---|---|---|
| 1 | `.promotional-banner__bg` (full-width-background mixin) | Promotional banner background pseudo | [_promotional-banner.scss:14](file:///Users/tri.nguyen/Project/aemaacs-investments-BE/aemaacs-investments/mandg-investments/ui.frontend/src/main/webpack/scss/base/6-components/promotional-banner/_promotional-banner.scss#L14) |
| 2 | `.strategy-hero__content` | Strategy hero content layer | [_strategy-hero.scss:40](file:///Users/tri.nguyen/Project/aemaacs-investments-BE/aemaacs-investments/mandg-investments/ui.frontend/src/main/webpack/scss/base/6-components/strategy-hero/_strategy-hero.scss#L40) |
| 3 | `.header-fixed::before` | Header fixed before pseudo (background) | [_header-base.scss:72](file:///Users/tri.nguyen/Project/aemaacs-investments-BE/aemaacs-investments/mandg-investments/ui.frontend/src/main/webpack/scss/base/6-components/mega-menu/_header-base.scss#L72) |
| 4 | `.hero-banner::after` (full-width-background) | Hero banner full width background | [_hero-banner.scss:295](file:///Users/tri.nguyen/Project/aemaacs-investments-BE/aemaacs-investments/mandg-investments/ui.frontend/src/main/webpack/scss/base/6-components/hero-banner/_hero-banner.scss#L295) |
| 5 | `.hero-banner-video__bg` | Hero banner video background | [_hero-banner-video.scss:55](file:///Users/tri.nguyen/Project/aemaacs-investments-BE/aemaacs-investments/mandg-investments/ui.frontend/src/main/webpack/scss/base/6-components/hero-banner/_hero-banner-video.scss#L55) |
| 6 | `.in-page-navigation__base` (2 lần) | In-page navigation base styles | [_in-page-navigation.scss:8,35](file:///Users/tri.nguyen/Project/aemaacs-investments-BE/aemaacs-investments/mandg-investments/ui.frontend/src/main/webpack/scss/base/6-components/in-page-navigation/_in-page-navigation.scss#L8) |
| 7 | `.in-page-navigation-top__base` | In-page navigation top base | [_in-page-navigation-top.scss:182](file:///Users/tri.nguyen/Project/aemaacs-investments-BE/aemaacs-investments/mandg-investments/ui.frontend/src/main/webpack/scss/base/6-components/in-page-navigation/_in-page-navigation-top.scss#L182) |
| 8 | `.article-header__base` | Article header base | [_article-header.scss:189](file:///Users/tri.nguyen/Project/aemaacs-investments-BE/aemaacs-investments/mandg-investments/ui.frontend/src/main/webpack/scss/base/6-components/article-header/_article-header.scss#L189) |
| 9 | `.slider-theme-style__base` | Slider theme style base | [_slider-theme-style.scss:62](file:///Users/tri.nguyen/Project/aemaacs-investments-BE/aemaacs-investments/mandg-investments/ui.frontend/src/main/webpack/scss/base/6-components/slider/_slider-theme-style.scss#L62) |
| 10 | `.fund-charge-calc .steps__base` | Calculator steps base | [_steps.scss:41](file:///Users/tri.nguyen/Project/aemaacs-investments-BE/aemaacs-investments/mandg-investments/ui.frontend/src/main/webpack/scss/base/6-components/fund-charge-calculator/components/_steps.scss#L41) |
| 11 | `.related-content-ampersands__base` | Related content ampersands base | [_related-content-ampersands.scss:29](file:///Users/tri.nguyen/Project/aemaacs-investments-BE/aemaacs-investments/mandg-investments/ui.frontend/src/main/webpack/scss/base/6-components/related-content/_related-content-ampersands.scss#L29) |

---

## ⚫ z: -1 — `$base-z-index-base-behind`

| # | Selector | Ngữ cảnh | File |
|---|---|---|---|
| 1 | `.swiper-slide::before` | Swiper slide pseudo background | [_swiper.scss:38](file:///Users/tri.nguyen/Project/aemaacs-investments-BE/aemaacs-investments/mandg-investments/ui.frontend/src/main/webpack/scss/base/3-generics/swiper/_swiper.scss#L38) |
| 2 | `.swiper-pagination` | Swiper pagination dots | [_swiper.scss:68](file:///Users/tri.nguyen/Project/aemaacs-investments-BE/aemaacs-investments/mandg-investments/ui.frontend/src/main/webpack/scss/base/3-generics/swiper/_swiper.scss#L68) |
| 3 | `.image__placeholder` | Image lazy load placeholder | [_image.scss:23](file:///Users/tri.nguyen/Project/aemaacs-investments-BE/aemaacs-investments/mandg-investments/ui.frontend/src/main/webpack/scss/base/6-components/image/_image.scss#L23) |
| 4 | `.strategy-hero__bg` | Strategy hero background image | [_strategy-hero.scss:60](file:///Users/tri.nguyen/Project/aemaacs-investments-BE/aemaacs-investments/mandg-investments/ui.frontend/src/main/webpack/scss/base/6-components/strategy-hero/_strategy-hero.scss#L60) |
| 5 | `.hero-banner__image` | Hero banner background image | [_hero-banner.scss:290](file:///Users/tri.nguyen/Project/aemaacs-investments-BE/aemaacs-investments/mandg-investments/ui.frontend/src/main/webpack/scss/base/6-components/hero-banner/_hero-banner.scss#L290) |
| 6 | `.header-fixed::after` | Header fixed after pseudo (backdrop overlay) | [_header-base.scss:85](file:///Users/tri.nguyen/Project/aemaacs-investments-BE/aemaacs-investments/mandg-investments/ui.frontend/src/main/webpack/scss/base/6-components/mega-menu/_header-base.scss#L85) |
| 7 | `.header-author::before` | Header author pseudo element | [_header-author.scss:29](file:///Users/tri.nguyen/Project/aemaacs-investments-BE/aemaacs-investments/mandg-investments/ui.frontend/src/main/webpack/scss/base/6-components/mega-menu/_header-author.scss#L29) |
| 8 | `.top-header-dropdown::before` | Top header dropdown backdrop | [_top-header-dropdown.scss:24](file:///Users/tri.nguyen/Project/aemaacs-investments-BE/aemaacs-investments/mandg-investments/ui.frontend/src/main/webpack/scss/base/6-components/mega-menu/top-header/_top-header-dropdown.scss#L24) |
| 9 | `.list-of-links__decoration` | List of links decorative element | [_list-of-links.scss:112](file:///Users/tri.nguyen/Project/aemaacs-investments-BE/aemaacs-investments/mandg-investments/ui.frontend/src/main/webpack/scss/base/6-components/list-of-links/_list-of-links.scss#L112) |
| 10 | `.button::before` (mixin) | Button pseudo element (hover background) | [_button.mixins.scss:31](file:///Users/tri.nguyen/Project/aemaacs-investments-BE/aemaacs-investments/mandg-investments/ui.frontend/src/main/webpack/scss/base/6-components/button/_button.mixins.scss#L31) |
| 11 | `.container::before` | Container pseudo element | [_container.scss:30](file:///Users/tri.nguyen/Project/aemaacs-investments-BE/aemaacs-investments/mandg-investments/ui.frontend/src/main/webpack/scss/base/6-components/container/_container.scss#L30) |
| 12 | `.in-page-navigation-left::before` (3 lần) | In-page left navigation pseudo elements | [_in-page-navigation-left.scss:85,266,339](file:///Users/tri.nguyen/Project/aemaacs-investments-BE/aemaacs-investments/mandg-investments/ui.frontend/src/main/webpack/scss/base/6-components/in-page-navigation/_in-page-navigation-left.scss#L85) |
| 13 | `.in-page-navigation-top::before` (2 lần) | In-page top navigation pseudo elements | [_in-page-navigation-top.scss:192,206](file:///Users/tri.nguyen/Project/aemaacs-investments-BE/aemaacs-investments/mandg-investments/ui.frontend/src/main/webpack/scss/base/6-components/in-page-navigation/_in-page-navigation-top.scss#L192) |
| 14 | `.related-content::before` | Related content pseudo | [_related-content.scss:289](file:///Users/tri.nguyen/Project/aemaacs-investments-BE/aemaacs-investments/mandg-investments/ui.frontend/src/main/webpack/scss/base/6-components/related-content/_related-content.scss#L289) |
| 15 | `.related-content-ampersands::before` | Related content ampersands pseudo | [_related-content-ampersands.scss:139](file:///Users/tri.nguyen/Project/aemaacs-investments-BE/aemaacs-investments/mandg-investments/ui.frontend/src/main/webpack/scss/base/6-components/related-content/_related-content-ampersands.scss#L139) |
| 16 | `.related-content-ampersands-listing::before` | Related content ampersands listing pseudo | [_related-content-ampersands-listing.scss:99](file:///Users/tri.nguyen/Project/aemaacs-investments-BE/aemaacs-investments/mandg-investments/ui.frontend/src/main/webpack/scss/base/6-components/related-content/_related-content-ampersands-listing.scss#L99) |

---

## Tổng kết nhanh

```
z:10000  ──  1 selector   (fullscreen overlay)
z: 9999  ──  3 selectors  (skip links, filter toggle mobile)
z: 1000  ──  8 selectors  (modals + header + banners) ⚠️ TRÙNG 2 TOKEN
z:  900  ──  1 selector   (popover)
z:  700  ──  1 selector   (navigation)
z:  600  ──  1 selector   (header label)
z:  500  ──  3 selectors  (sidebar)
z:  400  ──  3 selectors  (backdrop)
z:  300  ──  1 selector   (fixed)
z:  200  ──  4 selectors  (sticky)
z:  100  ──  6 selectors  (dropdown)
z:   10  ──  9 selectors  (elevated content)
z:    3  ──  9 selectors  (content L3)
z:    2  ── 18 selectors  (content L2)
z:    1  ── 24 selectors  (content L1)
z:    0  ── 11 selectors  (base)
z:   -1  ── 16 selectors  (behind/pseudo)
─────────────────────────
TỔNG   ── ~119 khai báo z-index
```
