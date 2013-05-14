####United States Metadata

**Where to Find Data**

The U.S. is currently in a transition period as federal agencies adapt to the new requirements of the [Managing Information as an Asset](http:/project-open-data.github.io) memo. On November, 9, 2013 you can access all federal government data at data.gov, and government data owned/maintained by specific federal agencies by going to *agency.gov*/data.json. Until then, much, but not all, government data will be available at these locations, described using the metadata below.

**Metadata Details**

Concept | Metadata | Required? | Cardinality | Description | Usage Notes
------- | -------- | ----- | ---- | ---------- | ---------
Title | title | Yes | (1,1) | Human-readable name of the asset. Should be in plain English and include sufficient detail to facilitate search and discovery. | string 
Description | description | Yes | (1,1) | Human-readable description (e.g., an abstract) with sufficient detail to enable a user to quickly understand whether the asset is of interest. | string
Keyword | keyword  | Yes  | (1,n)  | Tags (or keywords) help users discover your dataset, please include terms that would be used by technical and non-technical users. |   Separate keywords with commas.
Last Updated  | modified  | Yes  | (1,1)  | Most recent date on which the dataset was changed, updated or modified.  |  Dates should be formatted as YYYY-MM-DD. Specify “01” as the day if unknown. 
Organisation (Owner) | publisher  | Yes |  (1,1) |  The publishing agency. |   Departments and multi-unit agencies may use this field to describe which subordinate agency published this dataset.
Contact Person  | person | Yes | (1,1) | Contact person’s name for the asset.  |   Name should be formatted as Last, First
Contact Email  | mbox  | Yes | (1,1)  | Contact person’s email address.  |   Email address
Unique Identifier  | identifier  |  Yes | (1,1)  | A unique identifier for the dataset or API as maintained within an Agency catalog or database.  | This field allows third parties to maintain a consistent record for datasets even if title or URLs are updated. Agencies may integrate an existing system for maintaining unique identifiers or enter arbitrary characters for this field. However, each identifier must be unique across the agency’s catalog and remain fixed. Characters should be alphanumeric.
Public Access Level  | accessLevel  | Yes  | (1,1) |  The degree to which this dataset could be made publicly-available, regardless of whether it has been made available. Choices: Public (is or could be made publicly available), Restricted (available under certain conditions), or Private (never able to be made publicly available)  |   Must be one of the following: Public, Restricted, Private
Data Dictionary | dataDictionary  | If applicable  |(1,1) | URL to the data dictionary for the dataset or API. Note that documentation other than a Data Dictionary can be referenced using Related Documents as shown in the expanded fields.   |   URL
Download URL | accessURL  | If applicable  |  (1,1) |  URL providing direct access to the downloadable distribution of a dataset. |   This must be the direct download URL. Use **landingPage** for landing or disambiguation pages, or **references** for documentation pages.
API Endpoint |  webService |  If applicable | (1,)  | Endpoint of web service to access dataset.  |   This field will serve to delineate the web services offered by an agency and will be used to aggregate cross-government API catalogs.
Format | format | If applicable  | (0,1)  |  The file format or API type of the distribution. |   This must describe the exact file available at accessURL using file extensions (e.g., CSV, XLS, XSLX, TSV, JSON, XML). For example, if the download file is a ZIP containing a CSV, the entry here is “ZIP”.
License   | license  |  If applicable | (0,1)  | The license dataset or API is published with.  |   
Spatial Coverage | spatial  | If applicable  | (0,1)  | The range of spatial applicability of a dataset. Could include a spatial region like a bounding box or a named place.  |   This field should contain one of the following types of content: (1) a bounding coordinate box for the dataset represented in latitude / longitude pairs where the coordinates are specified in decimal degrees and in the order of: minimum longitude, minimum latitude, maximum longitude, maximum latitude; (2) a latitude / longitude pair (in decimal degrees) representing a point where the dataset is relevant; (3) a geographic feature expressed in Geography Markup Language using the Simple Features Profile; or (4) a geographic feature from the GeoNames database.
Temporal Coverage | temporal   | If applicable  | (0,1)  |  The range of temporal applicability of a dataset (i.e., a start and end date of applicability for the data). |   This field should contain an interval of time defined by start and end dates. Dates should be formatted as pairs of {start date, end date} in the format YYYY-MM-DD hh:mm:ss using 24 hour clock time notation (e.g., 2011-02-14 12:00:00, 2013-02-14 12:00:00).
Release Date    | issued  | No  | (0,1)  | Date of formal issuance.  |    Date (YYYY-MM-DD)
Frequency of Update  | accrualPeriodicity  |  No | (0,1)  |  Frequency with which dataset is published. |   Must be one of the following: hourly, daily, weekly, yearly, other
Language    | language  | No  | (0,n)  | The language of the dataset.  | string
Granularity    | granularity  | No  | (0,1)   | Level of granularity of the dataset.  |    Typically geographical or temporal.
Data Quality    | dataQuality | No  | (0,1)  |  Whether the dataset meets the agency’s Information Quality Guidelines. | Boolean (true/false)    
Category    | theme  |  No |  (0,n) |  Main thematic category of the dataset. |   Comma-separated values
Documentation | references  | No  | (0,n)  | Related documents such as technical information about a dataset, developer documentation, etc.  |   Comma-separated URLs
Size    | size  | No  | (0,1)  | The size of the downloadable dataset.  |   Sizes should be formatted as (e.g.), 52kb, 140mb, 2gb.
Homepage URL    |  landingPage |  No |(0,1) |  Alternative landing page used to redirect user to a contextual, Agency-hosted “homepage” for the Dataset or API when selecting this resource from the Data.gov user interface. |  URL; This field is not intended for an agency’s homepage (e.g. www.agency.gov), but rather if a dataset has a human-friendly hub or landing page that users should be directed to for all resources tied to the dataset. This allows agencies to better specify what a visitor receives after selecting one of the agency’s datasets on Data.gov or in third-party mashups.
RSS Feed | feed | No | (0,1) | URL for an RSS feed that provides access to the dataset. | URL; These RSS feeds will be used to create a cross-agency RSS feed search tool.
System of Records    | systemOfRecords  | No  | (0,1)  | URL to the System of Records related to this dataset.  |  URL


**Mappings to Other Vocabs**

Concept | Human-Readable Label | Metadata | CKAN | RDFa Lite 1.1 | Schema.org
------- | ----- | -------- | -------- | -------- | ----- | -------
Title | Title | title | title |  dcterms:title | sdo:name
Description | Description | description | notes | dcterms:description | sdo:description 
Keyword | Tags | keyword |  tags |  dcat:keyword |  sdo:keywords 
Last Updated  | Last Update  |  modified | revision_timestamp  |  dcterms:modified |  sdo:dateModified   
Organisation (Owner)  | Publisher  |  publisher | owner_org  | dcat:publisher  |  sdo:publisher
Contact Person  | Contact Name  | person  | maintainer  | foaf:person  |  sdo:person  
Contact Email  | Contact Email | mbox |  maintainer_email |  foaf:mbox |   -
Unique Identifier  | Unique Identifier  | identifier  |  id | dcterms:identifier   |  -   
Public Access Level  | Public Access Level  | accessLevel  | -  | -  | -   
Data Dictionary | Data Dictionary  |  dataDictionary |  dataDict |  dcat:dataDictionary | -   
Download URL | Download URL | accessURL  |  res_url | dcat:accessURL   |  sdo:contentUrl   
API Endpoint | Endpoint | webService  | res_url  |  dcat:webService* | sdo:url
Format |Format |  format|  res_format | dcterms:format  | sdo:encodingFormat   
License   | License   | license  | license_id   | dcterms:license  | -   
Spatial Coverage |  Spatial | spatial  | spatial |  dcterms:spatial | ds:spatialCoverage   
Temporal Coverage | temporal  | temporal  | -  | dcterms:temporal  |  ds:temporalCoverage   
Release Date    | Release Date  | issued  | -  |  dcterms:issued | sdo:datePublished   
Frequency of Update   | Frequency  |  accrualPeriodicity |  -|  dcterms:accrualPeriodicity | -  
Language    | Language  | language  | -  |  dcat:language | sdo:inLanguage  
Granularity    |  Granularity | granularity  | -  | dcat:granularity  | -   
Data Quality    | Data Quality  | dataQuality  | -  | xsd:boolean  |  -   
Category    | Category  | theme  | groups  |  dcat:theme |  sdo:about   
Documentation | Related Documents  |  references | resources |  dcterms:references | -   
Size    | Size  | size  | -  |  dcat:size | sdo:contentSize   
Homepage URL    | Homepage URL  | landingPage  |  url | dcat:landingPage  | sdo:url   
RSS Feed | RSS Feed  |feed | res_url | dcat:feed | sdo:url
System of Records    |  System of Records | systemOfRecords  | -  | -  |  -   

**Example JSON Excerpt**

[
    {
        "title": "Data Catalog",
        "description": "Version 1.0", 
        "keyword": "catalog", 
        "modified": "2013-05-09 06:00:00",
        "publisher": "US Department of X",
        "person": "Contact Person",
        "mbox": "contact.person@agency.gov",
        "identifier": "1",
        "accessLevel": "public",
        "distribution": [
            {
                "accessURL": "http://agency.gov/data.json",
                "format": "json"
            }
        ]  
    },
    {
        "title": "Public Elementary/Secondary Listing",
        "description": "The purpose of the CCD nonfiscal surveys is to provide a listing of all schools and agencies providing free public elementary and secondary education, along with basic descriptive statistical information on each school and agency listed. Penalties apply for misuse, seehttp://nces.ed.gov/ncesglobal/data_usage_agreement.aspfor more details.", 
        "keyword": "education, schools", 
        "modified": "2011-11-19 00:00:00",
        "publisher": "US Department of Education",
        "person": "Open Data Initiative",
        "mbox": "opendata@ed.gov",
        "identifier": "ykv5-fn9t",
        "accessLevel": "public",
        "dataDictionary": "http://nces.ed.gov/ccd/pdf/INsc09101a.pdf",
        "distribution": [
            {
                "accessURL": "https://explore.data.gov/views/ykv5-fn9t/rows.csv?accessType=DOWNLOAD", 
                "format": "csv",
                "size": "200mb"
            }, 
            {
                "accessURL": "https://explore.data.gov/views/ykv5-fn9t/rows.json?accessType=DOWNLOAD", 
                "format": "json"
            }, 
            {
                "accessURL": "https://explore.data.gov/views/ykv5-fn9t/rows.xml?accessType=DOWNLOAD", 
                "format": "xml"
            }
        ],
        "webService": "http://explore.data.gov/api/views/ykv5-fn9t/rows.json", 
        "license": "Public Domain", 
        "spatial": "US", 
        "temporal": "2009-09-01 00:00:00,2010-05-31 00:00:00", 
        "issued": "",
        "frequency": "one-time",
        "language": "English", 
        "granularity": "",
        "dataQuality": "true",
        "theme": "education", 
        "references": "http://nces.ed.gov/ccd/data/txt/psu091alay.txt", 
        "landingPage": "http://ed.gov/developer",
        "feed": "",
        "systemOfRecords": "http://nces.ed.gov/ccd/"     
    }]

