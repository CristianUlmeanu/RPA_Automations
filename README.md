# RPA_Automations

 A folder dedicated to multiple UiPath Automations that I've created and used in production for personal use, freelancing, or job clients that allowed me to share the automations.
 The automations are based on Robotic Enterprise Framework but in some cases, it was reinterpreted in an easier format because the automation wasn't that complicated or didn't use Orchestrator.
 The automations use all types of activities based on the needs of the process and also to be as compatible as possible for the platform it was used on.


## Costco Returns Extractor

This automation was created for the usage of an e-commerce brand that needed to process Costco's data of their returns. It has at its base the REF idea but it was implemented in a simpler way since it wasn't required full use of REF. The process includes the log-in and navigation of the Costco Wholesale website. It also gathers all the returns within a given time period and downloads them in PDF format locally. The PDFs are processed in order to extract all the information needed by the client, then it is stored into CSV format in order to be ready for upload into Netsuite. In the end, the PDFs are deleted since there wasn't a request in keeping it and provides an email at the end of the processing.

## Salesforce Product Change

The automation is used in the electric field. Based on a given input in CSV format, the automation is meant for changing the product of the input clients. It follows the REF, reads the input file, then logs in and navigates on the Salesforce platform. 90% of the actions are done strictly in the Salesforce platform since the process has to go through the website into each input client and follow a strict set of steps in order to change the client's energy contract.

## Cin7 Modify Moved Item Qty for Bulk Import CNs

This automation was created as a helper for the credit note bulk upload into Cin7. Because of the Cin7 CSV rules for bulk import for the credit notes, some of the fields that were mandatory for the client to be saved into the credit note were not allowed, so those fields needed to be manually modified after the bulk import. The automation logins into the website, navigates to the specific location where the credit notes are stored and based on a CSV file as input operates each of the input documents in order to complete the necessary fields for that credit note to be valid.

## Cin7 Void Duplicates

The automation is very close to a template for voiding duplicated entries. Because of the Cin7 friendly interface the automation was created and generalized in a manner that with a few changes can be used in voiding all types of documents from credit notes to invoices so it works very similar to a template. As the title suggests, the process logs into the platform, goes to the given category of documents, the last use was in credit notes, and voids the duplicated entries.

## Cin7 Update Sales Order

This automation is created again as a helper for the sales order bulk upload into Cin7. Because of the Cin7 CSV rules for bulk import for the sales order, some of the fields that were mandatory for the client to be saved into the sale order were not allowed, so those fields needed to be manually modified after the bulk import. The process uses an input CSV file for determining what documents need to be processed, and the fields that need to be modified. After reading the input, it logs into the platform navigates to the right category, and starts modifying the orders to match the information needed by the client.

## Discord Message Automation

The process is a very simple one it was created as a bot that writes random messages that were selected and added into an input file into a given discord group channel. It also randomises and makes sure to not retype the same thing over and over and also the typing is done in a random time window so it won't be detected by bot detectors that work on chat reading.

