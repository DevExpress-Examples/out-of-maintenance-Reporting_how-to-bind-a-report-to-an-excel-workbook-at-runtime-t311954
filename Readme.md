<!-- default badges list -->
![](https://img.shields.io/endpoint?url=https://codecentral.devexpress.com/api/v1/VersionRange/128598617/17.2.3%2B)
[![](https://img.shields.io/badge/Open_in_DevExpress_Support_Center-FF7200?style=flat-square&logo=DevExpress&logoColor=white)](https://supportcenter.devexpress.com/ticket/details/T311954)
[![](https://img.shields.io/badge/📖_How_to_use_DevExpress_Examples-e9f6fc?style=flat-square)](https://docs.devexpress.com/GeneralInformation/403183)
<!-- default badges end -->
<!-- default file list -->
*Files to look at*:

* [Form1.cs](./CS/BindingReportToExcelWorkbook/Form1.cs) (VB: [Form1.vb](./VB/BindingReportToExcelWorkbook/Form1.vb))
* [Program.cs](./CS/BindingReportToExcelWorkbook/Program.cs) (VB: [Program.vb](./VB/BindingReportToExcelWorkbook/Program.vb))
<!-- default file list end -->
# How to: Bind a Report to an Excel Workbook at runtime


<p>This code example demonstrates how to create a new blank report at runtime (an instance of the <strong>XtraReport</strong> class), bind it to a Microsoft Excel workbook, and then, fill the report with a <strong>DetailBand</strong> containing an <strong>XRLabel</strong> to show data from this workbook.</p>
<p>To bind a report to an Excel data source, create a new instance of the <strong>ExcelDataSource</strong> class and specify the full path to the source Excel file using the <strong>FileName</strong> property. Then, specify required settings used to extract data from the workbook and manually define the data source schema. Finally, assign the created data source to the report using the <strong>DataSource</strong> property.</p>
<p>In this example, an <strong>XRLabel</strong> is added to the report to display data of one data field.<br><br></p>
<p>Starting with v.17.2, the report uses <a href="https://documentation.devexpress.com/XtraReports/119236/Creating-Reports-in-Visual-Studio/Detailed-Guide-to-DevExpress-Reporting/Providing-Data-to-Reports/Data-Binding-Overview/Data-Binding-Modes">expression bindings</a> to provide data to controls. You can switch to the legacy binding mode by setting the <a href="https://documentation.devexpress.com/XtraReports/DevExpress.XtraReports.Configuration.UserDesignerOptions.DataBindingMode.property">UserDesignerOptions.DataBindingMode</a> property to <strong>Bindings </strong>at the application startup.</p>

<br/>


