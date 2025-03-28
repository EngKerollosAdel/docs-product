---
summary: OutSystems 11 (O11) enables data bootstrapping from Excel files into entities for efficient application development and testing.
tags: data import, entity management, excel integration, data bootstrapping, application development
locale: en-us
guid: b9f11658-2807-4efb-92ed-0413be0f2c63
app_type: traditional web apps, mobile apps, reactive web apps
platform-version: o11
figma:
audience:
  - mobile developers
  - frontend developers
  - full stack developers
outsystems-tools:
  - service studio
coverage-type:
  - apply
topic:
  - create-edit-entities
  - bootstrap-test-data-excel
---

# Bootstrap an Entity Using an Excel File

You can import data from an Excel file to load data to an entity. This is useful when you are developing and testing your application. This way, you can quickly have your data up and running in the application while developing it.

<div class="info" markdown="1">

If you're using Google Sheets, download your document as an .xlsx file (File > Download > Microsoft Excel), and then bootstrap the data. 
</div>

## Validate the Excel file

1. Open the Excel file, check that the Excel sheet has the name of the Entity and the column headers have the names of the entity attributes.

1. Close the Excel file. The bootstrap can't read the Excel file if it's open.

If your spreadsheet has blank cells and you're getting import errors, check [this How-to Guide](https://success.outsystems.com/Documentation/How-to_Guides/How_to_bootstrap_numeric_data_from_Excel_with_blank_cells) on how to proceed.

## Bootstrap the data

To bootstrap data from the first sheet of an Excel file to an existing entity, follow these steps:

1. In Service Studio, go to the Data tab, right-click on the entity and in the Advanced menu, choose 'Create Action to Bootstrap data from an Excel...'. 

1. Select the Excel file, check the mappings to see if they're correct and click on **Proceed**.
    Service Studio creates:

    * An action with the bootstrap logic named "Bootstrap&lt;entityname&gt;" in the Server Actions folder in the Logic tab.

    * A structure with the content of the Excel file named "Excel_&lt;filename&gt;" in the Structures folder in the Data tab.

    * A resource with the Excel file in the Resources folder in the Data tab.

    * A timer to execute the action at publish time named "Bootstrap&lt;entityname&gt;" in the Timers folder in the Processes tab.

1. Publish to bootstrap the data.

When you publish the module, it executes the action to bootstrap the data. If the entity already has data, the action with the bootstrap logic is **not** executed.

## Demo/Sample

Check this demo on how to bootstrap your data from an Excel file, and [download the Sample](resources/BootstrapFromExcel.oml) and the [sample data](resources/SampleData.xls) used in it.

<iframe src="https://player.vimeo.com/video/874767575" width="750" height="422" frameborder="0" allow="autoplay; fullscreen" allowfullscreen="">Video displaying how to bootstrap Entity data from Excel.</iframe>
