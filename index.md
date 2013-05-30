G8_Metadata_Mapping
===================

**Metadata Mapping Across G8 Members**

This page shows the mapping between the metadata on datasets published by G8 Membersthrough their open data portals. 

Below is an example of the mapping for the metadata term 'licence', i.e. the licence which specifies the terms underwhich a published open data set can be used.

This shows both the human-readable term (H) displayed to users of the portal (5.1H) as well as the machine-readable term (M) used in the technical backend of the portal, for developers (5.1M)

**Example of mapping - 'licence'**

 **Concepts** |**US**|**UK**|**France**|**Canada**|**EU**|**Germany**|**Japan**|**Italy**|**Russian Federation**|
-----|------|-----|-----|-----|-----|-----|------|-----|-----
5.1H Licence|license|Licence|Licence|Licence|Licence|Nutzungs- bestimmungen|ライセンス|Licenza|Условия использования набора данных|
5.1M License|license_id|License_id||Licence_id|License_id|License_id|License_id|field_Licenza||


**Detailed G8 metadata mapping**

The terms below have a number which is only used within this Github mapping. It allows you to understand where the same term is used between this index page and the more detailed explanation of metadata used by each Member. 

The index is as follows:

1. About the contact person, office or institution who has a role in relation to the data (e.g. owner, publisher, contact etc)

2. About the dataset (e.g. unique identifier, frequency of update, related keywords/tags etc)

3. Extent of the dataset (i.e. geographic area it covers e.g. period of time it covers, detail of data etc)

4. Supplemental information (i.e. other core useful information relating to the dataset/resource e.g. contextual documentation)

5. Distribution information (i.e. information relating to the resource e.g. size, format, language)

To go to a member's portal, click the link on the header row. (A.)

For more details about each member's schema, click the link to 'Detail'. (B.)

The general metadata concepts are listed in the left-hand column (A.)

 (A.)|[US](http://www.data.gov)|[UK](http://www.data.gov.uk)|[France](http://www.data.gouv.fr)|[Canada](http://www.data.gc.ca)|[EU](http://www.open-data.europa.eu/open-data)|[Germany](http://www.govdata.de)|[Japan](http:www.datameti.go.jp/data)|[Italy](http://www.dati.gov.it)|Russian Federation*
-----|------|-----|-----|-----|-----|-----|------|-----|-----
 **(B.)**|[US detail](/USmetadata.md)|UK detail|France detail|Canada detail|EU detail|Germany detail|Japan detail|Italy detail|RF detail - *currently no single portal
||
 **Concepts** |
*1. Contact Information*| | |
1.1 Contact Person|person|Editor|
1.2 Contact Email|mbox|Institution email|
1.3 Organisation (Owner)|publisher|Enquiries / FOI Contact|
Publisher|-||
Author| - |
Author Email| - |
Maintainer| - |
Maintainer Email| - |
*2. Dataset Information*| |
Unique Identifier|identifier|
Release Date|issued| 
Modified| - |
Last Updated|modified| 
Description|description| 
Keyword|keyword| 
Frequency of Update|accrual- Periodicity|
Title|title| 
Category | theme |
*3. Extent* | |
Spatial Coverage|spatial|
Spatial Type| - |
Spatial Coordinates| - |
Geographic Region Name| - |
Geographic Bounding Box - Lower Left Corner| - |
Bounding Box - Upper Right Corner| - |
Bounding Box - Coordinate Reference System| - |  
Geographic Bounding Box - Dimensions| - |
Temporal coverage|temporal|
Temporal coverage starts|temporal|
Temporal coverage ends|temporal|
Temporal granularity| - |
Temporal granularity factor| - |
Periodicity of data collection| - |
Periodicity of the production process| - |
Periodicity of the estimates| - |
Temporal and spatial comparability| - |
Periodicity of data dissemination| - |
Data quality|data- Quality|
Granularity|granularity|
*4. Supplemental Information* | |
Documentation|references|  
*5. Distribution Information* | |
Licence| |
Copyright| - |
Size | size | 
Download URL|access- URL|
Homepage URL|landing- Page|
Format|format|
Language|language|
Public Access Level|access- Level| 
API Endpoint|webService|
RSS Feed|feed|
Data Dictionary|data- Dictionary|
System of Records|systemOf- Records|


