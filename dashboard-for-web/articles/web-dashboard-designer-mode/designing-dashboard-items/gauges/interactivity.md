---
title: Interactivity
---
To enable interaction between the Gauge and other dashboard items, you can use the interactivity features, as **Master Filtering** and **Drill-Down**.
* [Master Filtering](#masterfiltering)
* [Drill-Down](#drilldown)

## <a name="masterfiltering"/>Master Filtering
You can use the **Gauge** dashboard item as a filter for other dashboard items. To learn more about filtering concepts common to all dashboard items, see the [Master Filtering](../../../../../dashboard-for-web/articles/web-dashboard-designer-mode/interactivity/master-filtering.md) topic.

When **Master Filtering** is enabled, you can click a gauge(s) to make other dashboard items only display data related to the selected gauge(s).

![Gauges_MasterFiltering_Web](../../../../images/Img22508.png)

To enable **Master Filtering**, go to the Gauge's [Interactivity](../../../../../dashboard-for-web/articles/web-dashboard-designer-mode/ui-elements/dashboard-item-menu.md) menu and select the required Master Filtering mode.

![wdd-dashboard-items-interactivity-section](../../../../images/Img125270.png)

To reset filtering, use the **Clear Master Filter** button (the ![wdd-master-filtering-icon](../../../../images/Img125072.png) icon) in the Gauge's [caption](../../../../../dashboard-for-web/articles/web-dashboard-designer-mode/dashboard-layout/dashboard-item-caption.md).

## <a name="drilldown"/>Drill-Down
The built-in drill-down capability allows you to change the detail level of data displayed in dashboard items on the fly. To learn more about drill-down concepts common to all dashboard items, see the [Drill-Down](../../../../../dashboard-for-web/articles/web-dashboard-designer-mode/interactivity/drill-down.md) topic.

When drill-down is enabled, you can click a gauge to view the details.

![Gauges_DrillDown_Web](../../../../images/Img22509.png)

Drill-down requires that the **Series** section contains several dimensions at the top, from the least detailed to the most detailed dimension.

![wdd-gauge-drill-down-arguments-section](../../../../images/Img125778.png)

> In OLAP mode, you can perform drill-down for either a hierarchy data item or several dimension attributes.

To enable **Drill-Down**, go to the Gauge's [Interactivity](../../../../../dashboard-for-web/articles/web-dashboard-designer-mode/ui-elements/dashboard-item-menu.md) menu and turn the **Drill-Down** option on.

![wdd-dashboard-items-interactivity-section](../../../../images/Img125270.png)

To return to the previous detail level, click the **Drill Up** button (the ![wdd-drill-up-icon](../../../../images/Img125074.png) icon) in the Gauge's [caption](../../../../../dashboard-for-web/articles/web-dashboard-designer-mode/dashboard-layout/dashboard-item-caption.md).