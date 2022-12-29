<!-- default badges list -->
![](https://img.shields.io/endpoint?url=https://codecentral.devexpress.com/api/v1/VersionRange/520094985/22.1.4%2B)
[![](https://img.shields.io/badge/Open_in_DevExpress_Support_Center-FF7200?style=flat-square&logo=DevExpress&logoColor=white)](https://supportcenter.devexpress.com/ticket/details/T1106334)
[![](https://img.shields.io/badge/📖_How_to_use_DevExpress_Examples-e9f6fc?style=flat-square)](https://docs.devexpress.com/GeneralInformation/403183)
<!-- default badges end -->

# Grid for Blazor - Disable Selection Checkboxes in Specific Rows

This example illustrates how to prevent users from selecting specific data items in the [DevExpress Grid for Blazor](https://docs.devexpress.com/Blazor/403143/grid). In this example, the Grid component disables the selection column's checkboxes for items, whose `Summary` field is set to `Mild`.

![Grid with Disabled Selection Checkbox](result.png)

Follow the steps below to allow users to select only the items that match your criteria:

1. Use the [DxGridSelectionColumn](https://docs.devexpress.com/Blazor/DevExpress.Blazor.DxGridSelectionColumn)'s [CellDisplayTemplate](https://docs.devexpress.com/Blazor/DevExpress.Blazor.DxGridSelectionColumn.CellDisplayTemplate) to replace the built-in checkbox with a custom [DxCheckBox](https://docs.devexpress.com/Blazor/DevExpress.Blazor.DxCheckBox-1) editor.

2. Create a lambda expression that checks whether the current data item matches your criteria. Assign this expression to the [Enabled](https://docs.devexpress.com/Blazor/DevExpress.Blazor.Base.DxDataEditorBase-2.Enabled) property of the checkbox.

3. Implement two-way data binding between the [Checked](https://docs.devexpress.com/Blazor/DevExpress.Blazor.DxCheckBox-1.Checked) property of the checkbox and the template context's [Selected](https://docs.devexpress.com/Blazor/DevExpress.Blazor.GridSelectionColumnCellDisplayTemplateContext.Selected) property.

## Files to Review

- [Index.razor](./CS/GridDisabledCheckboxes/Pages/Index.razor)

## Documentation

- [Selection Column](https://docs.devexpress.com/Blazor/DevExpress.Blazor.DxGridSelectionColumn)
- [Cell Display Template](https://docs.devexpress.com/Blazor/DevExpress.Blazor.DxGridSelectionColumn.CellDisplayTemplate)

## More Examples

- [Grid for Blazor - How to display detail information using DxFormLayout](https://github.com/DevExpress-Examples/blazor-DxGrid-Detail-Information-DxFormLayout)
- [Grid for Blazor - How to delete selected rows](https://github.com/DevExpress-Examples/blazor-dxgrid-delete-selected-rows)
