# mainwp-theming
MainWP is great tool - these customizations make it look the way you want

Just copy paste this CSS - the easy way is to instal WPCode snippet manager and add this as a CSS snippet and run it in 'admin area > admin header'
````
/* Theme CSS */
/* Define Variables */

:root {

  /* Sets color for primary button and text links. */
  --accent-color: #624ec1;

  /* Sets background color for the main navigation and top header elements. */
  --background-color-1: #000000;

  /* Sets background color for vertical menu, modal, accordion, sub-header, actions bar and segment elements. */
  --background-color-2: #111111;

  /* Sets background color for table headers, widgets, cards, modal headers and navigatoin wrapper elements. */
  --background-color-3: #111111;

  /* Sets background color for form field elements. */
  --background-color-4: #000000;

  /* Sets background color for table elements. */
  --table-background-color: #111111;

  /* Sets color for green elements. */
  --green-color: #624ec1;

  /* Sets color for yellow elements. */
  --yellow-color: #b09bfa;

  /* Sets color for red elements. */
  --red-color: #FFAB2A;

  /* Sets color for blue elements. */
  --blue-color: #b09bfa;

  /* Sets main text color. */
  --font-color: rgba(255, 255, 255, .9);

  /* Sets text color, lighter version. */
  --font-light-color: rgba(255, 255, 255, .7);

  /* Sets button text color. */
  --font-button-color: rgba(255, 255, 255, 1);

  /* Sets section element and table borders. */
  --border-color: rgba(255, 255, 255, .1);
}

/* Fix Colors */

.mainwp-ui.mainwp-custom-theme a:not(.ui.button),
.mainwp-ui.mainwp-custom-theme a:not(.ui.label, .uf-fmuci-button-main) {
  color: var(--accent-color);
}

.mainwp-ui.mainwp-custom-theme i.green.icon:not(.inverted) {
  color: var(--green-color) !important;
}

.mainwp-ui.mainwp-custom-theme .ui.green.label:not(.basic) {
  color: var(--font-button-color) !important;
  background-color: var(--green-color) !important;
}

.mainwp-ui.mainwp-custom-theme .ui.green.label.basic {
  color: var(--green-color) !important;
  border-color: var(--green-color) !important;
}

.mainwp-ui.mainwp-custom-theme i.red.icon:not(.inverted) {
  color: var(--red-color) !important;
}

.mainwp-ui.mainwp-custom-theme .ui.red.label:not(.basic) {
  color: var(--font-button-color) !important;
  background-color: var(--red-color) !important;
}

.mainwp-ui.mainwp-custom-theme #mainwp-version-label {
  background-color: var(--accent-color) !important;
}

.mainwp-ui.mainwp-custom-theme i.yellow.icon:not(.inverted) {
  color: var(--yellow-color) !important;
}

.mainwp-ui.mainwp-custom-theme .ui.yellow.label:not(.basic) {
  color: var(--font-button-color) !important;
  background-color: var(--yellow-color) !important;
}

.mainwp-ui.mainwp-custom-theme i.blue.icon:not(.inverted) {
  color: var(--blue-color) !important;
}

.mainwp-ui.mainwp-custom-theme .ui.blue.label:not(.basic) {
  color: var(--font-button-color) !important;
  background-color: var(--blue-color) !important;
}

.mainwp-ui.mainwp-custom-theme i.green.icon.inverted {
  color: var(--font-button-color) !important;
  background-color: var(--green-color) !important;
}

.mainwp-ui.mainwp-custom-theme i.red.icon.inverted {
  color: var(--font-button-color) !important;
  background-color: var(--red-color) !important;
}

.mainwp-ui.mainwp-custom-theme i.yellow.icon.inverted {
  color: var(--font-button-color) !important;
  background-color: var(--yellow-color) !important;
}

.mainwp-ui.mainwp-custom-theme i.blue.icon.inverted {
  color: var(--font-button-color) !important;
  background-color: var(--blue-color) !important;
}

.mainwp-ui.mainwp-custom-theme .ui.indeterminate.green.progress .bar::before,
.mainwp-ui.mainwp-custom-theme .ui.green.progress .bar,
.ui.progress .green.bar {
  background-color: var(--green-color) !important;
}

/* Invert Segments */

body.mainwp-ui.mainwp-custom-theme.pushable>.pusher,
body.mainwp-ui.mainwp-custom-theme,
.mainwp-ui.mainwp-custom-theme #wpbody-content,
.mainwp-ui.mainwp-custom-theme .mainwp-content-wrap,
.mainwp-ui.mainwp-custom-theme .ui.segment {
  background-color: var(--background-color-2) !important;
  color: var(--font-color);
}

.mainwp-ui.mainwp-custom-theme #mainwp-top-header {
  background: var(--background-color-1) !important;
  color: var(--font-color) !important;
  border: 0px solid var(--border-color) !important;
}
.mainwp-ui.mainwp-custom-theme #mainwp-top-header .ui.icon.button:not(.red, .green) {
  background: var(--background-color-3) !important;
  -webkit-box-shadow: inset 2px 0px 0px 1px var(--background-color-4) !important;
  -moz-box-shadow: inset 0px 0px 0px 1px var(--background-color-4) !important;
  box-shadow: inset 0px 0px 0px 1px var(--background-color-4) !important;
  color: var(--grey-light-alt) !important;
}
.mainwp-ui.mainwp-custom-theme #mainwp-page-navigation-wrapper {
  background-color: var(--background-color-3);
  padding: 0 !important;
  box-shadow: 0 1px 2px 0 rgba(0, 0, 0, .1) !important;
  border-top: 0px solid var(--border-color) !important;
  border-bottom: 1px solid var(--border-color) !important;
  border-left: 0px solid var(--border-color) !important;
  border-right: 1px solid var(--border-color) !important;
}

.mainwp-ui.mainwp-custom-theme #mainwp-page-navigation-wrapper .menu {
  margin-bottom: 0px !important;
  border-top: 0px solid var(--border-color) !important;
  border-bottom: 0px solid var(--border-color) !important;
  border-left: 0px solid var(--border-color) !important;
  border-right: 1px solid var(--border-color) !important;
  color: var(--font-color);
  background-color: var(--background-color-3);
}

.mainwp-ui.mainwp-custom-theme #mainwp-page-navigation-wrapper .menu .item {
  padding: 21px;
  color: var(--font-color);
}

.mainwp-ui.mainwp-custom-theme #mainwp-page-navigation-wrapper .menu .item.active,
.mainwp-ui.mainwp-custom-theme #mainwp-page-navigation-wrapper .menu .item:hover {
  background-color: var(--background-color-2);
  color: var(--accent-color);
}


.mainwp-ui.mainwp-custom-theme .mainwp-actions-bar,
.mainwp-ui.mainwp-custom-theme .mainwp-sub-header {
  border-bottom: 1px solid var(--border-color);
  background: var(--background-color-2);
}

.mainwp-ui.mainwp-custom-theme .mainwp-side-content,
.mainwp-ui.mainwp-custom-theme .mainwp-main-content {
  border-color: var(--border-color) !important;
}

.mainwp-ui.mainwp-custom-theme #mainwp-sites-menu-sidebar .mainwp-site-menu-item .title {
  color: var(--font-color) !important;
}

/* Headers */

.mainwp-ui.mainwp-custom-theme h2,
.mainwp-ui.mainwp-custom-theme h2.header {
  color: var(--font-color);
}

.mainwp-ui.mainwp-custom-theme h3,
.mainwp-ui.mainwp-custom-theme h3.header {
  color: var(--font-color);
}

.mainwp-ui.mainwp-custom-theme h4,
.mainwp-ui.mainwp-custom-theme h4.header {
  color: var(--font-color);
}

/* Invert Side Bar */

.mainwp-ui.mainwp-custom-theme #mainwp-select-sites-header .ui.menu {
  border-color: var(--border-color);
}

.mainwp-ui.mainwp-custom-theme #mainwp-select-sites-header .ui.menu a.item {
  color: var(--font-color);
}

.mainwp-ui.mainwp-custom-theme #mainwp-select-sites-header .ui.menu a.item.active {
  color: var(--accent-color);
}

.mainwp-ui.mainwp-custom-theme #mainwp-select-sites .ui.divided.list .item {
  border-color: var(--border-color) !important;
}

.mainwp-ui.mainwp-custom-theme .ui.list .item {
  color: var(--font-color) !important;
  border-color: var(--border-color) !important;
}

.mainwp-ui.mainwp-custom-theme .ui.list .item .header,
.mainwp-ui.mainwp-custom-theme .ui.list .item .description {
  color: var(--font-color) !important;
}

.mainwp-ui.mainwp-custom-theme .ui.selection.list .item {
  color: var(--font-color) !important;
  border-color: var(--border-color) !important;
}

.mainwp-ui.mainwp-custom-theme #mainwp-select-sites .ui.divided.list .item label {
  color: var(--font-color) !important;
}

.mainwp-ui.mainwp-custom-theme #mainwp-select-sites-select-all-actions {
  background-color: var(--border-color);
  border-color: var(--border-color);
}

.mainwp-ui.mainwp-custom-theme .mainwp-side-content .title {
  color: var(--font-color) !important;
}

.mainwp-ui.mainwp-custom-theme .mainwp-sidebar-options {
  background-color: var(--background-color-2);
}

/* Invert Widgets */

.mainwp-ui.mainwp-custom-theme .ui.segment.mainwp-widget {
  background-color: var(--background-color-3);
  border-color: var(--border-color) !important;
  color: var(--font-color);
}

.mainwp-ui.mainwp-custom-theme .ui.segment.mainwp-widget .ui.header,
.mainwp-ui.mainwp-custom-theme .ui.segment.mainwp-widget .ui.header .sub.header,
.mainwp-ui.mainwp-custom-theme .ui.segment.mainwp-widget .statistic .label,
.mainwp-ui.mainwp-custom-theme .ui.segment.mainwp-widget .statistic .value {
  color: var(--font-color);
}

.mainwp-ui.mainwp-custom-theme .ui.segment.mainwp-widget .ui.horizontal.divider {
  border-color: var(--border-color);
  color: var(--font-color);
}

.mainwp-ui.mainwp-custom-theme .ui.segment.mainwp-widget .ui.list .item .content .header,
.mainwp-ui.mainwp-custom-theme .ui.segment.mainwp-widget .ui.list .item .content .description,
.mainwp-ui.mainwp-custom-theme .ui.segment.mainwp-widget .ui.list .item {
  border-color: var(--border-color);
  color: var(--font-color);
}

.mainwp-ui.mainwp-custom-theme .mainwp-no-results-placeholder {
  opacity: .2;
}

/* Invert Tables */

.mainwp-ui.mainwp-custom-theme .ui.table,
.mainwp-ui.mainwp-custom-theme .ui.inverted.table {
  background: var(--table-background-color);
  color: var(--font-color);
}

.mainwp-ui.mainwp-custom-theme .ui.table tr th,
.mainwp-ui.mainwp-custom-theme .ui.inverted.table tr th {
  background-color: var(--background-color-3);
  border-color: var(--border-color);
  color: var(--font-color);
}

.mainwp-ui.mainwp-custom-theme table tr th.settinglabel {
  border-color: var(--border-color);
  color: var(--font-color);
}

.mainwp-ui.mainwp-custom-theme .ui.definition.table>thead>tr>th:first-child {
  background-color: var(--background-color-3);
  border-color: var(--border-color);
  color: var(--font-color);
  box-shadow: none !important;
}

.mainwp-ui.mainwp-custom-theme .ui.table tr td {
  border-color: var(--border-color);
}

.mainwp-ui table.dataTable tbody tr>.dtfc-fixed-left,
.mainwp-ui table.dataTable tbody tr>.dtfc-fixed-right {
  background-color: var(--table-background-color) !important;
}

.mainwp-ui.mainwp-custom-theme .ui.definition.table>tbody>tr>td:first-child:not(.ignored) {
  color: var(--font-color);
}

.mainwp-ui.mainwp-custom-theme .ui.table tr.hoverli {
  background-color: var(--background-color-4) !important;
}

.mainwp-ui.mainwp-custom-theme .ui.table tr.active {
  background-color: var(--background-color-4) !important;
}

.mainwp-ui.mainwp-custom-theme .ui.table tr.active td {
  color: var(--font-color) !important;
}


.mainwp-ui.mainwp-custom-theme .ui.selection.table tr:hover td,
.mainwp-ui.mainwp-custom-theme .ui.selectable.table tr:hover td {
  color: var(--font-light-color);
}

.mainwp-ui.mainwp-custom-theme .alternate,
.mainwp-ui.mainwp-custom-theme .striped>tbody> :nth-child(2n+1) {
  background-color: var(--background-color-3);
}

.mainwp-ui.mainwp-custom-theme #mainwp-manage-themes-table tbody tr td:first-child,
.mainwp-ui.mainwp-custom-theme #mainwp-manage-plugins-table tbody tr td:first-child {
  background-color: var(--background-color-3);
}

.mainwp-ui.mainwp-custom-theme .ui.table tbody tr.positive,
.mainwp-ui.mainwp-custom-theme #mainwp-manage-themes-table tbody tr td.positive,
.mainwp-ui.mainwp-custom-theme #mainwp-manage-plugins-table tbody tr td.positive {
  background-color: rgba(127, 177, 0, .1) !important;
  color: var(--font-color) !important;
}

.mainwp-ui.mainwp-custom-theme .ui.table tbody tr.error,
.mainwp-ui.mainwp-custom-theme .ui.table tbody tr.negative,
.mainwp-ui.mainwp-custom-theme #mainwp-manage-themes-table tbody tr td.negative,
.mainwp-ui.mainwp-custom-theme #mainwp-manage-plugins-table tbody tr td.negative {
  background-color: rgba(160, 0, 0, .1) !important;
  color: var(--font-color) !important;
}


.mainwp-ui.mainwp-custom-theme .ui.table tbody tr.warning,
.mainwp-ui.mainwp-custom-theme #mainwp-manage-themes-table tbody tr td.warning,
.mainwp-ui.mainwp-custom-theme #mainwp-manage-plugins-table tbody tr td.warning {
  background-color: rgba(181, 129, 5, .1) !important;
  color: var(--font-color) !important;
}

.mainwp-ui.mainwp-custom-theme #mainwp-manage-updates table tr.active,
.mainwp-ui.mainwp-custom-theme #mainwp-manage-updates table tr.ui.title.active {
  background: var(--background-color-3) !important;
}

.mainwp-ui.mainwp-custom-theme #mainwp-manage-updates table tr.content.active {
  background: var(--background-color-3) !important;
}

.mainwp-ui.mainwp-custom-theme #mainwp-manage-updates table tr.content.active table tfoot tr th,
.mainwp-ui.mainwp-custom-theme #mainwp-manage-updates table tr.content.active table thead tr th {
  background: var(--background-color-2) !important;
  color: var(--font-color) !important;
}

.mainwp-ui.mainwp-custom-theme #mainwp-manage-updates table tr.content.active table tbody tr td {
  background: var(--background-color-2) !important;
  color: var(--font-color) !important;
}

.mainwp-ui.mainwp-custom-theme #mainwp-plugins-content .mainwp-manage-plugin-item,
.mainwp-ui.mainwp-custom-theme #mainwp-themes-content .mainwp-manage-theme-item {
  border-bottom: 1px solid var(--border-color) !important;
}

.mainwp-ui.mainwp-custom-theme #mainwp-plugins-content .mainwp-manage-plugin-item-website,
.mainwp-ui.mainwp-custom-theme #mainwp-themes-content .mainwp-manage-theme-item-website {
  background: var(--background-color-3) !important;
  color: var(--font-color) !important;
  border-bottom: 1px solid var(--border-color) !important;
  border-top: 1px solid var(--border-color) !important;
}

.mainwp-ui.mainwp-custom-theme table.dataTable.table > tbody > tr.selected > * {
  color: var(--font-color);
}

/* Invert Form Fields */

.mainwp-ui.mainwp-custom-theme .ui.tab textarea,
.mainwp-ui.mainwp-custom-theme .ui.form textarea {
  background-color: var(--background-color-4);
  border-color: var(--border-color);
  color: var(--font-color);
}

.mainwp-ui.mainwp-custom-theme .ui.input>input {
  background-color: var(--background-color-4);
  border-color: var(--border-color);
  color: var(--font-color);
}

.mainwp-ui.mainwp-custom-theme .ui.input input[disabled] {
  color: var(--font-light-color);
}

.mainwp-ui.mainwp-custom-theme .ui.tab input,
.mainwp-ui.mainwp-custom-theme .ui.form input,
.mainwp-ui.mainwp-custom-theme .ui.form select,
.mainwp-ui.mainwp-custom-theme .ui.dropdown.selection {
  background: var(--background-color-4);
  color: var(--font-color);
  border-color: var(--border-color);
}



.mainwp-ui.mainwp-custom-theme .ui.form input:focus,
.mainwp-ui.mainwp-custom-theme .ui.form select:focus,
.mainwp-ui.mainwp-custom-theme .ui.dropdown.selection:focus {
  background-color: var(--background-color-4);
  color: var(--font-color);
}

.mainwp-ui.mainwp-custom-theme .ui.form .field label {
  color: var(--font-color);
}

.mainwp-ui.mainwp-custom-theme .ui.input .ui.basic.label {
  color: var(--font-light-color);
  background-color: var(--background-color-4);
  border-color: var(--border-color);
}

.mainwp-ui.mainwp-custom-theme .ui.header,
.mainwp-ui.mainwp-custom-theme .ui.header .sub.header {
  color: var(--font-color);
}

.mainwp-ui.mainwp-custom-theme .ui.dividing.header {
  border-color: var(--border-color);
}

.mainwp-ui.mainwp-custom-theme .ui.toggle.checkbox.checked label::before,
.mainwp-ui.mainwp-custom-theme .ui.slide.checkbox.checked label::before {
  background: var(--green-color) !important;
}

.mainwp-ui.mainwp-custom-theme .ui.toggle.checkbox label::before,
.mainwp-ui.mainwp-custom-theme .ui.slide.checkbox label::before {
  color: var(--font-color);
  background: var(--background-color-4);
}

.mainwp-ui.mainwp-custom-theme .ui.checkbox input~label,
.mainwp-ui.mainwp-custom-theme .ui.radio.checkbox input~label {
  color: var(--font-color) !important;
}

.mainwp-ui.mainwp-custom-theme .ui.checkbox.checked input~label,
.mainwp-ui.mainwp-custom-theme .ui.radio.checkbox.checked input~label {
  color: var(--font-color) !important;
}

.mainwp-ui.mainwp-custom-theme .ui.checkbox input~label::before,
.mainwp-ui.mainwp-custom-theme .ui.radio.checkbox input~label::before {
  background: var(--background-color-4) !important;
  color: var(--font-color) !important;
  border-color: var(--border-color);
}

.mainwp-ui.mainwp-custom-theme .ui.checkbox.checked input~label::before,
.mainwp-ui.mainwp-custom-theme .ui.radio.checkbox.checked input~label::before {
  background: var(--accent-color) !important;
}

.mainwp-ui.mainwp-custom-theme .ui.checkbox input~label::after,
.mainwp-ui.mainwp-custom-theme .ui.radio.checkbox input~label::after {
  color: var(--font-color) !important;
}

.mainwp-ui.mainwp-custom-theme .ui.checkbox.checked input~label::after,
.mainwp-ui.mainwp-custom-theme .ui.radio.checkbox.checked input~label::after {
  color: var(--background-color-2) !important;
}

.mainwp-ui.mainwp-custom-theme .ui.radio.checkbox input~label::after {
  background-color: var(--font-color) !important;
}

.mainwp-ui.mainwp-custom-theme .ui.radio.checkbox.checked input~label::after {
  background-color: var(--background-color-2) !important;
}

.mainwp-ui.mainwp-custom-theme .ui.field input.labelauty+label {
  background-color: var(--background-color-2) !important;
}

.mainwp-ui.mainwp-custom-theme .mainwp-managesites-import-rows:nth-of-type(odd) {
  background-color: rgba(255, 255, 255, .06) !important;
}

/* Invert Messages */

.mainwp-ui.mainwp-custom-theme .ui.message .header {
  color: var(--font-color);
}

.mainwp-ui.mainwp-custom-theme .ui.message {
  color: var(--font-color);
  background-color: var(--background-color-4);
  box-shadow: none;
  -webkit-box-shadow: none;
}

.mainwp-ui.mainwp-custom-theme .ui.info.message {
  color: var(--font-color);
  background-color: var(--blue-color);
  box-shadow: none;
  -webkit-box-shadow: none;
}

.mainwp-ui.mainwp-custom-theme .ui.red.message {
  color: var(--font-color);
  background-color: var(--red-color);
  box-shadow: none;
  -webkit-box-shadow: none;
}

.mainwp-ui.mainwp-custom-theme .ui.yellow.message {
  color: var(--font-color);
  background-color: var(--yellow-color);
  box-shadow: none;
  -webkit-box-shadow: none;
}

.mainwp-ui.mainwp-custom-theme .ui.green.message {
  color: var(--font-color);
  background-color: var(--green-color);
  box-shadow: none;
  -webkit-box-shadow: none;
}

.mainwp-ui.mainwp-custom-theme .ui.message a {
  color: var(--font-color) !important;
  font-weight: bolder;
}

/* Invert Cards */

.mainwp-ui.mainwp-custom-theme .ui.cards .card {
  background-color: var(--background-color-3);
  border: 1px solid var(--border-color) !important;
  color: var(--font-color);
  box-shadow: none;
  -webkit-box-shadow: none;
}

.mainwp-ui.mainwp-custom-theme .ui.cards .card .description,
.mainwp-ui.mainwp-custom-theme .ui.cards .card .meta {
  color: var(--font-color);
}

.mainwp-ui.mainwp-custom-theme .ui.cards .card .meta a {
  color: var(--accent-color);
}

.mainwp-ui.mainwp-custom-theme .ui.cards .card .header {
  color: var(--font-color);
}

.mainwp-ui.mainwp-custom-theme .ui.cards .card .content {
  border-top: 1px solid var(--border-color) !important;
  color: var(--font-color);
}

.mainwp-ui.mainwp-custom-theme .ui.cards .card .extra a:not(.ui) {
  color: var(--accent-color);
}

/* Invert Steps */

.mainwp-ui.mainwp-custom-theme .ui.steps .step {
  background-color: var(--background-color-3) !important;
}

.mainwp-ui.mainwp-custom-theme .ui.steps .step .description {
  color: var(--font-color) !important;
}

/* Invert Feed */

.mainwp-ui.mainwp-custom-theme .ui.feed .summary {
  color: var(--font-color) !important;
}

.mainwp-ui.mainwp-custom-theme .ui.feed .summary .date {
  color: var(--font-light-color) !important;
}

/* Invert Modal */

.mainwp-ui.mainwp-custom-theme .ui.modal i.icon.close {
  top: 0.8em;
  right: 0.8em;
  color: #ffffff;
  opacity: 1 !important;
  text-shadow: none !important;
}

.mainwp-ui.mainwp-custom-theme .ui.modal>.header,
.mainwp-ui.mainwp-custom-theme .ui.modal>.actions {
  background: var(--background-color-3);
  border-color: var(--border-color);
  color: var(--font-color);
}

.mainwp-ui.mainwp-custom-theme .ui.modal,
.mainwp-ui.mainwp-custom-theme .ui.modal>.content {
  background: var(--background-color-2);
  border-color: var(--border-color);
  color: var(--font-color);
}

.mainwp-ui.mainwp-custom-theme .ui.progress .label {
  color: var(--font-color);
}

.mainwp-ui.mainwp-custom-theme .ui.modal .ui.list .item {
  border-color: var(--border-color);
  color: var(--font-color);
}

.mainwp-ui.mainwp-custom-theme .ui.modal .ui.list .item .content,
.mainwp-ui.mainwp-custom-theme .ui.list .item .content {
  color: var(--font-color);
}

/* Invert Labels */

.mainwp-ui.mainwp-custom-theme .ui.label:not(.green),
.mainwp-ui.mainwp-custom-theme .ui.label:not(.basic),
.mainwp-ui.mainwp-custom-theme .ui.label:not(.disabled),
.mainwp-ui.mainwp-custom-theme .ui.label:not(.red) {
  background-color: var(--background-color-1);
  border: 1px solid var(--table-background-color);
  color: var(--font-light-color);
  box-shadow: none;
  -webkit-box-shadow: none;
}

.mainwp-ui.mainwp-custom-theme .ui.basic.label {
  background: none !important;
}

/* Invert Buttons and Icons */

.mainwp-ui.mainwp-custom-theme .icon {
  color: var(--font-color);
}

.mainwp-ui.mainwp-custom-theme a:not(.button) .icon:not(.green, .red) {
  color: var(--accent-color);
}

.mainwp-ui.mainwp-custom-theme .ui.button:not(.green),
.mainwp-ui.mainwp-custom-theme .ui.button:not(.basic),
.mainwp-ui.mainwp-custom-theme .ui.button:not(.disabled),
.mainwp-ui.mainwp-custom-theme .ui.button:not(.red) {
  background-color: var(--background-color-1);
  border: 1px solid var(--table-background-color);
  color: var(--font-light-color);
  box-shadow: none;
  -webkit-box-shadow: none;
}

.mainwp-ui.mainwp-custom-theme .ui.button[disabled],
.mainwp-ui.mainwp-custom-theme .ui.button.disabled {
  background-color: var(--table-background-color) !important;
  border: none !important;
  color: rgba(255, 255, 255, .3);
  box-shadow: none !important;
  -webkit-box-shadow: none !important;
}

.mainwp-ui.mainwp-custom-theme .ui.button.green:not(.basic),
.mainwp-ui.mainwp-custom-theme .ui.button.green:not(.disabled),
.mainwp-ui.mainwp-custom-theme .ui.button.green:not(.red) {
  background-color: var(--accent-color);
  color: var(--font-color);
  border: none;
  box-shadow: none;
  -webkit-box-shadow: none;
}

.mainwp-ui.mainwp-custom-theme .ui.button.green.basic {
  background-color: var(--background-color-1);
  color: var(--accent-color);
  -webkit-box-shadow: inset 0px 0px 0px 1px var(--accent-color);
  -moz-box-shadow: inset 0px 0px 0px 1px var(--accent-color);
  box-shadow: inset 0px 0px 0px 1px var(--accent-color);
}

.mainwp-ui.mainwp-custom-theme .ui.button.red {
  background-color: var(--red-color);
}

.mainwp-ui.mainwp-custom-theme .ui.button.green.basic .icon {
  color: var(--accent-color);
}

.mainwp-ui.mainwp-custom-theme .mainwp-nav-wrap .icon {
  color: var(--font-color) !important;
}


.mainwp-ui.mainwp-custom-theme button.mainwp-sites-select-select-button,
.mainwp-ui.mainwp-custom-theme button.mainwp-sites-select-deselect-button {
  color: var(--font-button-color);
}

/* Invert Dimmer */

.mainwp-ui.mainwp-custom-theme .ui.inverted.dimmer {
  background: var(--background-color-2);
  opacity: .9;
}

.mainwp-ui.mainwp-custom-theme .ui.inverted.dimmer .text {
  color: var(--font-light-color);
}

/* Invert Menus */

.mainwp-ui.mainwp-custom-theme .ui.dropdown .menu {
  background-color: var(--background-color-4);
}

.mainwp-ui.mainwp-custom-theme .ui.dropdown .menu:after {
  background: var(--background-color-4) !important;
}

.mainwp-ui.mainwp-custom-theme .ui.dropdown .menu .item {
  color: var(--font-color);
  border-color: var(--border-color) !important;
}

.mainwp-ui.mainwp-custom-theme .ui.dropdown .menu .item.active,
.mainwp-ui.mainwp-custom-theme .ui.dropdown .menu .item.selected,
.mainwp-ui.mainwp-custom-theme .ui.dropdown .menu .item:hover {
  background-color: var(--background-color-3) !important;
}

.mainwp-ui.mainwp-custom-theme #mainwp-first-level-navigation {
  background-color: var(--background-color-1);
}

.mainwp-ui.mainwp-custom-theme #mainwp-second-level-navigation,
.mainwp-ui.mainwp-custom-theme #mainwp-second-level-navigation .ui.inverted.menu {
  background-color: var(--background-color-3);
}

.mainwp-ui.mainwp-custom-theme #mainwp-sites-sidebar-menu.ui.vertical.menu {
  background-color: var(--background-color-2);
}

.mainwp-ui.mainwp-custom-theme .ui.pointing.vertical.menu {
  background-color: var(--background-color-3);
  border-color: var(--border-color) !important;
}

.mainwp-ui.mainwp-custom-theme #mainwp-sites-sidebar-menu.ui.vertical.menu .item {
  border-bottom: 1px solid var(--border-color) !important;
}

.mainwp-ui.mainwp-custom-theme #mainwp-sites-sidebar-menu.ui.vertical.menu .item:last-child {
  border-bottom: none !important;
}

.mainwp-ui.mainwp-custom-theme #mainwp-sites-sidebar-menu.ui.vertical.menu .item a .label,
.mainwp-ui.mainwp-custom-theme #mainwp-sites-sidebar-menu.ui.vertical.menu .item a,
.mainwp-ui.mainwp-custom-theme #mainwp-sites-sidebar-menu.ui.vertical.menu .item .icon {
  color: var(--font-color) !important;
}

.mainwp-ui.mainwp-custom-theme .ui.pointing.vertical.menu .item {
  border-color: var(--border-color);
  color: var(--font-color);
}

.mainwp-ui.mainwp-custom-theme #mainwp-sites-sidebar-menu.ui.vertical.menu .item:hover,
.mainwp-ui.mainwp-custom-theme .ui.pointing.vertical.menu .item:hover {
  background-color: var(--background-color-4);
}

.mainwp-ui.mainwp-custom-theme #mainwp-sites-sidebar-menu.ui.vertical.menu .item.active,
.mainwp-ui.mainwp-custom-theme .ui.pointing.vertical.menu .item.active {
  border-color: var(--border-color);
  background-color: var(--background-color-4);
  color: var(--font-color);
}

.mainwp-ui.mainwp-custom-theme #mainwp-sites-sidebar-menu.ui.vertical.menu .item:after,
.mainwp-ui.mainwp-custom-theme .ui.pointing.vertical.menu .item:after {
  display: none !important;
}

.mainwp-ui.mainwp-custom-theme .mainwp-api-icon {
  color: var(--accent-color);
}

.mainwp-ui.mainwp-custom-theme .ui.pagination.menu {
  background-color: var(--background-color-3);
  border-color: var(--border-color);
}
.mainwp-ui.mainwp-custom-theme .ui.pagination.menu .item.disabled .page-link {
  color: var(--font-light-color) !important;
}
.mainwp-ui.mainwp-custom-theme .ui.pagination.menu .item:hover,
.mainwp-ui.mainwp-custom-theme .ui.pagination.menu .item.active {
  background: var(--accent-color);
}
.mainwp-ui.mainwp-custom-theme .ui.pagination.menu .item:hover .page-link,
.mainwp-ui.mainwp-custom-theme .ui.pagination.menu .item.active .page-link {
  color: var( --background-color-3 );
}

/* Invert Placeholder */

.mainwp-ui.mainwp-custom-theme .ui.placeholder {
  opacity: 0.02;
}

/* Accordion */

.mainwp-ui.mainwp-custom-theme .mainwp-content-wrap .ui.accordion .title,
.mainwp-ui.mainwp-custom-theme .mainwp-content-wrap .ui.accordion .content {
  color: var(--font-color);
  border-color: var(--border-color) !important;
  background-color: var(--background-color-2) !important;
}

.mainwp-ui.mainwp-custom-theme .ui.accordion .title:hover {
  color: var(--font-color) !important;
}

.mainwp-ui.mainwp-custom-theme .ui.accordion .content.active label {
  color: var(--font-color) !important;
}

/* Invert Editor */

.mainwp-ui.mainwp-custom-theme #wp-content-editor-tools {
  background-color: var(--background-color-2) !important;
}

.mainwp-ui.mainwp-custom-theme #post-status-info {
  background: var(--background-color-2);
  border: 0px solid var(--background-color-2) !important;
}

/* Invert Calendar */

.mainwp-ui.mainwp-custom-theme .ui.calendar {
  background-color: var(--table-background-color) !important;
}

.mainwp-ui.mainwp-custom-theme .ui.calendar:before {
  background-color: var(--table-background-color) !important;
}

/* Yoast SEO Widget */

.mainwp-ui.mainwp-custom-theme #wpseo_meta.postbox {
  background: var(--background-color-2);
  border: 0px solid var(--background-color-2) !important;
}

/* WP Widget */

.mainwp-ui.mainwp-custom-theme .widget-inside,
.mainwp-ui.mainwp-custom-theme .widget-top {
  background: var(--background-color-2);
  border: 1px solid var(--border-color);
}


.mainwp-ui.mainwp-custom-theme #ngBulkSettingsManagerId {
  background: var(--background-color-2) !important;
}

/* Buddy Support */
.mainwp-ui.mainwp-custom-theme .profile_box {
  background: var(--background-color-2);
  border: 1px solid var(--border-color);
  color: var(--font-color);
  box-shadow: none !important;
}

.mainwp-ui.mainwp-custom-theme .profile_box .bb-remote-checkbox {
  border-top: 1px solid var(--border-color);
}

.mainwp-ui.mainwp-custom-theme .profile_item_select,
.mainwp-ui.mainwp-custom-theme .profile_item_noselect,
.mainwp-ui.mainwp-custom-theme .profile_settings {
  background: var(--background-color-3);
  border: 1px solid var(--border-color);
}

.mainwp-ui.mainwp-custom-theme .form-table th {
  color: var(--font-color);
}


.mainwp-ui.mainwp-custom-theme .form-table td input,
.mainwp-ui.mainwp-custom-theme .form-table td select,
.mainwp-ui.mainwp-custom-theme .form-table td a.button {
  background-color: var(--background-color-4) !important;
  color: var(--font-color);
}

/* Apexcharts */

.mainwp-ui.mainwp-custom-theme .apexcharts-menu {
  background: var(--background-color-3) !important;
  border-color: var(--border-color) !important;
}

.mainwp-ui.mainwp-custom-theme .apexcharts-menu .apexcharts-menu-item:hover {
  background: var(--background-color-4) !important;
}

.mainwp-ui.mainwp-custom-theme.mainwp_page_InsightsOverview .ui.segment.mainwp-widet {
  color: #eee !important;
}

/* Wordfence Support */

.mainwp-ui.mainwp-custom-theme .wf-block {
  background: var(--background-color-3) !important;
  border: 1px solid var(--border-color);
}

.mainwp-ui.mainwp-custom-theme .wf-scan-results {
  border-color: var(--border-color) !important;
}

.mainwp-ui.mainwp-custom-theme .wf-scan-tabs {
  box-shadow: none !important;
}

.mainwp-ui.mainwp-custom-theme .wf-block-list li,
.mainwp-ui.mainwp-custom-theme #wf-scan-results-new {
  border-color: var(--border-color) !important;
}

.mainwp-ui.mainwp-custom-theme .wf-scan-tabs li.wf-tab {
  background-color: var(--background-color-3) !important;
  color: var(--font-color) !important;
  border: none !important;
}

.mainwp-ui.mainwp-custom-theme #wf-scan-bulk-buttons-delete,
.mainwp-ui.mainwp-custom-theme #wf-scan-bulk-buttons-repair {
  background-color: var(--accent-color) !important;
  color: var(--font-color) !important;
  border: none !important;
}

.mainwp-ui.mainwp-custom-theme .wf-scanner-progress>.wf-scan-step>.wf-scan-step-icon>.wf-scan-step-disabled,
.mainwp-ui.mainwp-custom-theme .wf-scanner-progress>.wf-scan-step>.wf-scan-step-icon>.wf-scan-step-premium,
.mainwp-ui.mainwp-custom-theme .wf-scanner-progress>.wf-scan-step>.wf-scan-step-icon>.wf-scan-step-pending,
.mainwp-ui.mainwp-custom-theme .wf-scanner-progress>.wf-scan-step>.wf-scan-step-icon>.wf-scan-step-running,
.mainwp-ui.mainwp-custom-theme .wf-scanner-progress>.wf-scan-step>.wf-scan-step-icon>.wf-scan-step-complete-success,
.mainwp-ui.mainwp-custom-theme .wf-scanner-progress>.wf-scan-step>.wf-scan-step-icon>.wf-scan-step-complete-warning {
  background-color: var(--background-color-3) !important;
}

.mainwp-ui.mainwp-custom-theme .wf-scanner-progress>.wf-scan-step:first-of-type,
.mainwp-ui.mainwp-custom-theme .wf-scanner-progress>.wf-scan-step:last-of-type {
  background: var(--background-color-3) !important;
}

.mainwp-ui.mainwp-custom-theme .wf-issue:nth-of-type(2n),
.mainwp-ui.mainwp-custom-theme .wf-issue-site-cleaning:nth-of-type(2n) {
  background-color: var(--background-color-3) !important;
}

.mainwp-ui.mainwp-custom-theme .wf-issue,
#wf-scan-activity-log .wf-issue-site-cleaning {
  border-color: var(--border-color) !important;
}

.mainwp-ui.mainwp-custom-theme #wf-scan-activity-log {
  background-color: var(--background-color-3) !important;
}

/* dark theme */
.mainwp-ui.mainwp-custom-theme .dt-scroll-body tbody tr.selected .ui.red.button,
.mainwp-ui.mainwp-custom-theme .dt-scroll-body tbody tr.selected .ui.basic.red.button,
.mainwp-ui.mainwp-custom-theme .dt-scroll-body tbody tr.selected .ui.button.green,
.mainwp-ui.mainwp-custom-theme .dt-scroll-body tbody tr.selected .ui.button.basic.green{
  color: #fff !important;
}
/* end */


/*******************************
         Scrollbars
*******************************/

/* For WebKit Browsers (e.g., Chrome, Edge, Safari) */
::-webkit-scrollbar {
  width: 5px; /* Width of the scrollbar */
}

::-webkit-scrollbar-track {
  background: #1c1d1b; /* Background of the track */
}

::-webkit-scrollbar-thumb {
  background-color: #FFAB2A; /* Color of the scrollbar thumb */
  border-radius: 5px; /* Round edges for the thumb */
  border: 2px solid #1c1d1b; /* Optional: creates padding between thumb and track */
}

::-webkit-scrollbar-thumb:hover {
  background: #FFAB2A; /* Thumb color on hover */
}

/* For Firefox (using CSS Scrollbars Module Level 1) */
* {
  scrollbar-width: thin; /* Options: auto, thin */
  scrollbar-color: #FFAB2A #1c1d1b; /* thumb color, track color */
}

/* Extra CSS */
#mainwp-first-level-navigation-menu .item.active .icon, #mainwp-first-level-navigation-menu .item.active .text {
    color: #ffffff !important;
}
span.ui.green.text {
    color: #b09bfa !important;
}
#mainwp-second-level-navigation .ui.inverted.menu .item .item:hover, #mainwp-second-level-navigation .ui.inverted.menu .item .item.active {
    color: #624ec1 !important;
}
span.ui.red.text {
    color: #FFAB2A !important;
}
.ui.indeterminate.red.progress .bar::before, .ui.red.progress .bar, .ui.progress .red.bar {
    background-color: #FFAB2A !important;
}
#mainwp-main-menu {
    width: 100%;
    background: #000000 !important;
}
#mainwp-first-level-navigation-menu {
    background: #000000 !important;
}

#mainwp-first-level-navigation-menu .item.active {
    background: #624ec1 !important;
}
.ui.inverted.menu .active.item {
    background: #111111 !important;
}
.mainwp-ui.mainwp-custom-theme #mainwp-second-level-navigation, .mainwp-ui.mainwp-custom-theme #mainwp-second-level-navigation .ui.inverted.menu {
    background-color: #000000 !important;
}
#mainwp-collapse-second-level-navigation {
    background-color: #000000;
}
