G8_Metadata_Mapping
===================

**Metadata Mapping Across G8 Members**

This page shows the mapping between the metadata on datasets published by G8 Members through their open data portals. 

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

'H' denotes the 'human-readable' label; 'M' the 'machine-readable' label. 

The metadata relates to datasets, unless the index number also has an 'R' in brackets, in which case it refers to a 'resource'.

To go to a member's portal, click the link on the header row. (A.)

For more details about each member's schema, click the link to 'Detail'. (B.)

The general metadata concepts are listed in the left-hand column (A.)

 (A.)|[US](http://www.data.gov)|[UK](http://www.data.gov.uk)|[France](http://www.data.gouv.fr)|[Canada](http://www.data.gc.ca)|[EU](http://www.open-data.europa.eu/open-data)|[Germany](http://www.govdata.de)|[Japan](http:www.datameti.go.jp/data)|[Italy](http://www.dati.gov.it)|Russian Federation*
-----|------|-----|-----|-----|-----|-----|------|-----|-----
 **(B.)**|[US detail](/USmetadata.md)|UK detail|France detail|Canada detail|EU detail|Germany detail|Japan detail|Italy detail|RF detail - *currently no single portal
||
 **Concepts** |
*1. Contact Information*| | |
1.1H Person|Contact Name||
1.1M Person|maintainer||
1.2 Contact Email|mbox|Institution email|
1.3 Organisation (Owner)|publisher|Enquiries / FOI Contact|
1.4 Publisher|-||
1.5 Author| - |
1.6 Author Email| - |
1.7 Maintainer| - |
1.8 Maintainer Email| - |
*2. Dataset Information*| |
2.1 Unique Identifier|identifier|
2.2 Release Date|issued| 
2.3 Modified| - |
2.4 Last Updated|modified| 
2.5 Description|description| 
2.6 Keyword|keyword| 
2.7 Frequency of Update|accrual- Periodicity|
2.8 Title|title| 
2.9 Category | theme |
*3. Extent* | |
3.1 Spatial Coverage|spatial|
3.2 Spatial Type| - |
3.3 Spatial Coordinates| - |
3.4 Geographic Region Name| - |
3.5 Geographic Bounding Box - Lower Left Corner| - |
3.6 Bounding Box - Upper Right Corner| - |
3.7 Bounding Box - Coordinate Reference System| - |  
3.8 Geographic Bounding Box - Dimensions| - |
3.9 Temporal coverage|temporal|
3.10 Temporal coverage starts|temporal|
3.11 Temporal coverage ends|temporal|
3.12 Temporal granularity| - |
3.13 Temporal granularity factor| - |
3.14 Periodicity of data collection| - |
3.15 Periodicity of the production process| - |
3.16 Periodicity of the estimates| - |
3.17 Temporal and spatial comparability| - |
3.18 Periodicity of data dissemination| - |
3.19 Data quality|data- Quality|
3.20 Granularity|granularity|
*4. Supplemental Information* | |
4.1 Documentation|references|  
*5. Distribution Information* | |
5.1 Licence| |
5.2 Copyright| - |
5.3 Size | size | 
5.4 Download URL|access- URL|
5.5 Homepage URL|landing- Page|
5.6 Format|format|
5.7 Language|language|
5.8 Public Access Level|access- Level| 
5.9 API Endpoint|webService|
5.10 RSS Feed|feed|
5.11 Data Dictionary|data- Dictionary|
5.12 System of Records|systemOf- Records|

**Feedback**
Please give feedback on this mapping - you can fill out a [short survey (5 questions)](http://www.surveymonkey.com/s/CCM3F2C) or a longer one (10 questions).
