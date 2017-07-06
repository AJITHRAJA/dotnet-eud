---
title: Query Builder
---
# Query Builder
In the **Query Builder** dialog, you can add data tables and views to the data source, and select which columns to include. The **Query Builder** automatically joins the related tables, so all you need to do is drag-and-drop.

![wdd-query-builder](../../../../images/Img124934.png)

This topic consists of the following sections.
* [Add Tables](#add)
* [Join Tables](#join)
* [Edit Column Settings](#edit)
* [Filter Data](#filter)
* [Preview Data](#preview)

## <a name="add"/>Add Tables
To add the required tables/views to a data source, drag-and-drop it from the **Tables** pane onto the **Diagram** pane.

![wdd-query-builder-add-table](../../../../images/Img125656.png)

Then, select the required columns.

![wdd-quey-builder-select-column](../../../../images/Img125657.png)

To delete the unnecessary table, select it and click the **Delete** button (the ![wdd-query-builder-delete-icon](../../../../images/Img125661.png) icon).

You can cancel or repeat the action using the **Undo**/**Redo** buttons (the ![wdd-query-builder-undo](../../../../images/Img126299.png) and ![wdd-query-builder-redo](../../../../images/Img126300.png) icons).

## <a name="join"/>Join Tables
When you drop a table that has a relationship at the database level with any of the recently added tables, the **Query Builder** joins these tables automatically.

![wdd-query-builder-join-tables](../../../../images/Img125658.png)

You can create a relationship between two tables manually by dragging a column in one table to a related column in a different table. A relationship line will be drawn between the two tables.

![wdd-query-builder-join-tables-manually](../../../../images/Img125659.png)

The Query Builder allows you to change the join type (if necessary). For this, select the relationship line and use the **Join type** combo box in the Properties pane. An **Inner join** and **Left outer join** are supported.

![wdd-query-builder-ralstionship-properties](../../../../images/Img125660.png)

To delete the unnecessary relationship, select the relationship line and click the **Delete** button (the ![wdd-query-builder-delete-icon](../../../../images/Img125661.png) icon).

## <a name="edit"/>Edit Column Settings
To edit a column setting, select the required column in a table. Then, use the **Properties** pane to specify the column setting.

The following settings are available for each column.

![wdd-queru-builder-properties-pane](../../../../images/Img124947.png)
* The **Name** field displays the selected column name.
* The **Type** field displays the selected column type.
* The **Alias** field allows you to specify the column alias.
	
	> Note that aggregated columns should always have an alias.
* The **Output** field allows you to choose whether to include the selected column to the query.
* Use **Sort Type** to specify the sort order of column values.
* The **Sort Order** field allows you to specify the order in which several columns are sorted.
* The **Group By** option allows you to group data by the values of the selected column.
* The **Aggregate** field allows you to specify the aggregate function used to aggregate column values.
	
	> Note that you should apply aggregation/grouping either to all columns or to none of them.

## <a name="filter"/>Filter Data
The Query Builder allows you to filter a query. To do this, deselect tables and click the ellipsis button in the appeared **Filter** field in the **Properties** pane. This invokes the **Filter Editor** dialog, which provides a visual interface for constructing a filter string.

![wdd-filter-editor-filter-query](../../../../images/Img124905.png)

To learn more, see [Filter Queries](../../../../../dashboard-for-web/articles/web-dashboard-designer-mode/providing-data/working-with-sql-data-sources/filter-queries.md).

## <a name="preview"/>Preview Data
The Query Builder allows you to preview data for the created SQL query. To do this, click the **Preview Results...** button. This invokes the [Data Preview](../../../../../dashboard-for-web/articles/web-dashboard-designer-mode/providing-data/working-with-sql-data-sources/preview-data.md) window containing data returned after executing the query.