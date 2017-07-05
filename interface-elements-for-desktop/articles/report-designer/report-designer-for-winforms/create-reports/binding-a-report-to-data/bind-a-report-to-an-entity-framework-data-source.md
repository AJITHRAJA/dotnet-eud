---
title: Bind a Report to an Entity Framework Data Source
---
This document describes the steps required to connect a report to data provided by an Entity Framework data context.

To bind a report to an Entity Framework data source, do the following.
1. [Create a new report](../../../../../../interface-elements-for-desktop/articles/report-designer/report-designer-for-winforms/create-reports/basic-operations/create-a-new-report.md).
2. Click the report's [Smart Tag](../../../../../../interface-elements-for-desktop/articles/report-designer/report-designer-for-winforms/report-designer-reference/report-designer-ui/smart-tag.md). In the invoked actions list, expand  the **Data Source** drop-down list and click **Add New DataSource**.
	
	![RD_CreateReports_BindReport_0](../../../../../images/Img8330.png)
3. The first page of the invoked **Data Source Wizard** allows you to specify the data source type. Select **Entity Framework** and click **Next** to proceed.
	
	![RD_CreateReports_BindReport_EFDataSource_SelectDatasourceType](../../../../../images/Img23810.png)
4. On the next page, select the required data context from the list of available data contexts and click **Next**.
	
	![RD_ReportWizard_EFSelectDataContext](../../../../../images/Img23794.png)
5. Select a connection string to be used to establish a data connection.
	
	![RD_ReportWizard_EFSelectConnectionString](../../../../../images/Img23795.png)
	
	Click **Next** to proceed to the next page.
6. The following wizard page is available only if the current entity data model contains stored procedures. To bind to a stored procedure, click **Add**. Then, in the invoked window, select a required stored procedure and click **OK**.
	
	![RD_ReportWizard_EFBindToStoredProcedure](../../../../../images/Img23796.png)
7. Configure the parameters to be passed to the selected stored procedure. Be sure to specify the correct parameter **Type**. Click **Finish** to exit the wizard.
	
	![RD_DataSourceWizard_EF_StoredProcedure](../../../../../images/Img122139.png)

The newly created Entity Framework data source will be displayed in the **Components** node of the [Report Explorer](../../../../../../interface-elements-for-desktop/articles/report-designer/report-designer-for-winforms/report-designer-reference/report-designer-ui/report-explorer.md). Additionally, the hierarchy of the data source will be reflected by the [Field List](../../../../../../interface-elements-for-desktop/articles/report-designer/report-designer-for-winforms/report-designer-reference/report-designer-ui/field-list.md).

![RD_CreateReports_BindReport_EFDataSource_ReportExplorer](../../../../../images/Img23812.png)