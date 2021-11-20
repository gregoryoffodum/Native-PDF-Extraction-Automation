# Native-PDF-Extraction-Automation
extract relevant fields from different pdf variants

![](invoice_demo.gif)

## Objective

The bot classifies and extracts relevant information from native *.pdf receipts and invoices from email attachments using UiPath studio

## Scope

- Robotic Process Automation
- Intelligent Automation
- UiPath
- Regular Expressions

## Input Files

- The [Attachments](https://github.com/gregoryoffodum/Native-PDF-Extraction-Automation/tree/main/attachments) folder houses the attachments after email automation (extracted from email attachments). 

- The [Regular Expression](https://github.com/gregoryoffodum/Native-PDF-Extraction-Automation/blob/main/regex.xlsx) file contains the regex syntax for all the invoice variants. It was an input in the loop (**Match** activity) to extract selected fields and populate the results in an adjacent column. These values are subsequently moved to a datatable and exported as an excel file. 

## Methodology
 
The [Process Definition Document](https://github.com/gregoryoffodum/Native-PDF-Extraction-Automation/blob/main/Process%20Definition%20Document%20(PDD).docx) describes the As-Is and To-Be methodologies accordingly. 
Key activities: 
- Excel Scope 
- Select Case
- Get IMAP mail messages
- Read PDF Text
- For Each
- Build Datatable
- Match

## Process
- [Flowchart](https://github.com/gregoryoffodum/Native-PDF-Extraction-Automation/blob/main/receiptRobot.drawio) summarizes the process flow of the To-Be framework.
- [Main](https://github.com/gregoryoffodum/Native-PDF-Extraction-Automation/blob/main/Main.xaml) is the main bot xaml file to be run by UiPath. All processes are embedded therein with clear annotations and descriptions.

## Output File

[Receipt](https://github.com/gregoryoffodum/Native-PDF-Extraction-Automation/blob/main/receipt.xlsx) is the exported file and result of the automation robot.
