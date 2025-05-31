# Migration TODOs: Angular to Vue

This file tracks the status of porting each component from Angular to Vue. **Whenever a component's status changes, this file MUST be updated.**

## Migration Status Table

| Component | Status |
|-----------|--------|
| aside/aside.component | Not Started |
| autocomplete/autocomplete.component | Not Started |
| calendar/calendar.component | Not Started |
| calendar/month-select/month-select.component | Not Started |
| calendar/month-view/month-view.component | Not Started |
| calendar/year-select/year-select.component | Not Started |
| color-picker/color-input.component | Not Started |
| color-picker/color-picker.component | Not Started |
| color-picker/color-swatch.component | Not Started |
| common/option/optgroup.component | Not Started |
| common/option/option.component | Not Started |
| common/selection/pseudo-checkbox/pseudo-checkbox.component | Not Started |
| common/typography/base/base-text.component | Not Started |
| common/typography/caption/caption.component | Not Started |
| common/typography/label/label.component | Not Started |
| common/typography/link/link.component | Not Started |
| common/typography/text/text.component | Not Started |
| common/typography/title/title.component | Not Started |
| data-table/cell-headers/data-table-checkbox-header-cell.component | Not Started |
| data-table/cell-headers/data-table-expand-header-cell.component | Not Started |
| data-table/cell-headers/data-table-header-cell-filter-header.component | Not Started |
| data-table/cell-headers/data-table-header-cell.component | Not Started |
| data-table/cells/data-table-cell.component | Not Started |
| data-table/cells/data-table-checkbox-cell.component | Not Started |
| data-table/cells/data-table-expand-cell.component | Not Started |
| data-table/data-table-clear-button.component | Not Started |
| data-table/data-table.component | Not Started |
| data-table/pagination/data-table-pagination.component | Not Started |
| data-table/rows/data-table-header-row.component | Not Started |
| data-table/rows/data-table-row.component | Not Started |
| data-table/sort-filter/sort-button.component | Not Started |
| divider/divider.component | Not Started |
| field/toggle/picker-toggle.component | Not Started |
| form/extras/number-range/number-range.component | Not Started |
| layout/container/layout-container.component | Not Started |
| layout/content/layout-content.component | Not Started |
| layout/rail/rail.component | Not Started |
| layout/sidenav/sidenav.component | Not Started |
| menu/menu-content.component | Not Started |
| menu/menu.component | Not Started |
| modal/modal-container.component | Not Started |
| modal/modal.component | Not Started |
| places/places.component | Not Started |
| query-builder/condition-builder/condition-builder.component | Not Started |
| query-builder/condition-group/condition-group.component | Not Started |
| query-builder/condition-templates/condition-templates.component | Not Started |
| query-builder/criteria-builder/criteria-builder.component | Not Started |
| select-search/select-search.component | Not Started |
| stepper/step-header.component | Not Started |
| stepper/step-label.component | Not Started |
<!-- Add more components as needed -->

---

## Migration Sections

### Aside
- `aside/aside.component.ts`

### Autocomplete
- `autocomplete/autocomplete.component.ts`

### Calendar
- `calendar/calendar.component.ts`
- `calendar/month-select/month-select.component.ts`
- `calendar/month-view/month-view.component.ts`
- `calendar/year-select/year-select.component.ts`

### Color Picker
- `color-picker/color-input.component.ts`
- `color-picker/color-picker.component.ts`
- `color-picker/color-swatch.component.ts`

### Common/Option
- `common/option/optgroup.component.ts`
- `common/option/option.component.ts`

### Common/Selection
- `common/selection/pseudo-checkbox/pseudo-checkbox.component.ts`

### Common/Typography
- `common/typography/base/base-text.component.ts`
- `common/typography/caption/caption.component.ts`
- `common/typography/label/label.component.ts`
- `common/typography/link/link.component.ts`
- `common/typography/text/text.component.ts`
- `common/typography/title/title.component.ts`

### Data Table
- `data-table/cell-headers/data-table-checkbox-header-cell.component.ts`
- `data-table/cell-headers/data-table-expand-header-cell.component.ts`
- `data-table/cell-headers/data-table-header-cell-filter-header.component.ts`
- `data-table/cell-headers/data-table-header-cell.component.ts`
- `data-table/cells/data-table-cell.component.ts`
- `data-table/cells/data-table-checkbox-cell.component.ts`
- `data-table/cells/data-table-expand-cell.component.ts`
- `data-table/data-table-clear-button.component.ts`
- `data-table/data-table.component.ts`
- `data-table/pagination/data-table-pagination.component.ts`
- `data-table/rows/data-table-header-row.component.ts`
- `data-table/rows/data-table-row.component.ts`
- `data-table/sort-filter/sort-button.component.ts`

### Divider
- `divider/divider.component.ts`

### Field
- `field/toggle/picker-toggle.component.ts`

### Form/Extras
- `form/extras/number-range/number-range.component.ts`

### Layout
- `layout/container/layout-container.component.ts`
- `layout/content/layout-content.component.ts`
- `layout/rail/rail.component.ts`
- `layout/sidenav/sidenav.component.ts`

### Menu
- `menu/menu-content.component.ts`
- `menu/menu.component.ts`

### Modal
- `modal/modal-container.component.ts`
- `modal/modal.component.ts`

### Places
- `places/places.component.ts`

### Query Builder
- `query-builder/condition-builder/condition-builder.component.ts`
- `query-builder/condition-group/condition-group.component.ts`
- `query-builder/condition-templates/condition-templates.component.ts`
- `query-builder/criteria-builder/criteria-builder.component.ts`

### Select Search
- `select-search/select-search.component.ts`

### Stepper
- `stepper/step-header.component.ts`
- `stepper/step-label.component.ts`

<!-- Add more sections/components as you discover them -->

---

## Project Overview Rule

**Rule:** Whenever a component is ported or its migration status changes, you must update `TODO.md` to reflect the new status. This ensures the migration progress is always up to date and visible to all contributors.
