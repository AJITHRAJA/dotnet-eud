---
title: Creating Calculated Fields
---
The Dashboard Designer provides the capability to create calculated fields that allow you to apply complex expressions to data fields that are obtained from the dashboard's data source. You can use these fields in data visualizations as regular data source fields.
* [Creating a Calculated Field](#creating-a-calculated-field)
* [Editing a Calculated Field](#editing-a-calculated-field)

> Note that calculated fields are not supported for [OLAP](../../../../dashboard-for-desktop/articles/dashboard-designer/providing-data/connecting-to-olap-cubes.md) data sources.

## <a name="creating-a-calculated-field"/>Creating a Calculated Field
After you have created a data source, you can add a new calculated field based on the existing data source fields.

To create a calculated field, select the required data source (and the required [query](../../../../dashboard-for-desktop/articles/dashboard-designer/working-with-data/manage-sql-queries.md)/data member, if applicable) in the [Data Source Browser](../../../../dashboard-for-desktop/articles/dashboard-designer/ui-elements/data-source-browser.md) and click the **Add Calculated Field** button in the Ribbon's Data Source tab...

![CalculatedFileds_AddCalculatedFieldButton_Ribbon](../../../images/Img21578.png)

...or right-click the Field List and select **Add Calculated Field** in the context menu.

![CalculatedFileds_AddCalculatedField_ContextMenu](../../../images/Img21581.png)

This invokes the [Expression Editor](../../../../dashboard-for-desktop/articles/expression-editor.md) dialog, which allows you to specify an expression that will be used to obtain calculated field values. Here, you can construct the required expression.

![CalculatedFileds_ExpressionEditor](../../../images/Img21580.png)

You can use the following elements in expressions.
* Functions
	
	> To learn how to use **Aggregate** functions, see [Aggregations](../../../../dashboard-for-desktop/articles/dashboard-designer/data-analysis/aggregations.md). The [Expression Operators, Functions and Constants](../../../../dashboard-for-desktop/articles/expression-editor/expression-operators-functions-and-constants.md) topic lists common functions (**DateTime**, **Math**, **String**, etc.) supported by expressions.
* Operators
* Columns
* Constants
* [Parameters](../../../../dashboard-for-desktop/articles/dashboard-designer/data-analysis/using-dashboard-parameters.md)

After the expression has been specified, click **OK**. This displays a new calculated field in the data source structure.

![CalculatedFileds_DataSourceStructure](../../../images/Img21582.png)

Now you can specify the required calculated field type, change its default name, etc.

## <a name="editing-a-calculated-field"/>Editing a Calculated Field
To edit a calculated field, use its context menu.

![CalculatedFileds_FieldContextMenu](../../../images/Img21583.png)

This menu contains the following items.

| Item | Description |
|---|---|
| **Edit Expression...** | Invokes the [Expression Editor](../../../../dashboard-for-desktop/articles/expression-editor.md) dialog, which allows you to change an expression for an existing calculated field. |
| **Field Type** | Specifies the type of the calculated field. |
| **Rename** | Changes the calculated field name. |
| **Delete** | Removes the existing calculated field from the data source. |