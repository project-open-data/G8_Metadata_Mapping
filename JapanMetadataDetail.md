####Japan Metadata

**Metadata Details**

Concept|Description|Front-end (human-readable)|National metadata schema|Back-end machine-readable|Required|Data Type|Format: pattern|Cardinality|Usage Notes
------- | -------- | ----- | ---- | ---------- | ---------|-------|-------|-------|------
1 *Contact information*|||||||||
1.1 Person	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|
1.2 Contact Email - Publisher	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|
1.2 Contact Email - Dataset	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|
1.3 Organisation (Owner)	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|
1.4 Publisher	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|
1.5 Author	|	-	|	作成者 	|	-	|	author	|	No	|	See Usage Notes	|	See Usage Notes	|	(0,1)	|	Name should be formatted as First, Last in Japanese.	|
1.6 Author Email	|	-	|	作成者のメールアドレス	|	-	|	author_email	|	No	|	email-address	|	-	|	(0,1)	|	-	|
1.7 Maintainer	|	-	|	メンテナー	|	-	|	mainainer	|	No	|	See Usage Notes	|	See Usage Notes	|	(0,1)	|	Name should be formatted as First, Last in Japanese.	|
1.8 Maintainer Email	|	-	|	メンテナーのメールアドレス	|	-	|	maintainer_email	|	No	|	email-address	|	-	|	(0,1)	|	-	|
2. *Dataset Identification*	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|
2.1 Unique Identifier	|	-	|	URLの一部	|	-	|	name	|	Yes	|	-	|	-	|	(1,1)	|	-	|
2.2 Release Date	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|
2.2.R Release Date	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|
2.3 Modified	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|
2.3.R Modified	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|
2.4 Last Updated	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|
2.4.R Last Updated	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|
2.5 Description	|	-	|	説明	|	-	|	notes	|	No	|	string	|	-	|	(0,1)	|	-	|
2.6 Keyword	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|
2.7 Frequency of Update	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|
2.8 Title	|	-	|	タイトル	|	-	|	title	|	Yes	|	string	|	-	|	(1,1)	|	-	|
2.9 Category	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|
3 *Extent Information*	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|
3.1 Spatial coverage	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|
3.2 Spatial Type	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|
3.3 Spatial Coordinates	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|
3.4 Geographic Region Name	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|
3.5 Geographic Bounding Box - Lower Left Corner  	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|
3.6 Bounding Box - Upper Right Corner  	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|
3.7 Bounding Box - Coordinate Reference System  	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|
3.8 Geographic Bounding Box - Dimensions  	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|
3.9 Temporal coverage	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|
3.10 Temporal coverage starts	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|
3.11 Temporal coverage ends	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|
3.12 Temporal granularity	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|
3.13 Temporal granularity factor	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|
3.14 Periodicity of data(set) collection	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|
3.15 Periodicity of the production process	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|
3.16 Periodicity of the estimates	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|
3.17 Temporal and spatial comparability	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|
3.18 Periodicity of data dissemination	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|
3.19 Data quality	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|
3.20.X Reference period	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|
4. *Supplemental Information*	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|
4.1 Documentation URL - resource	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|
5. *Distribution Information*	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|
5.1 Licence	|	-	|	ライセンス	|	-	|	license_id	|	Yes	|	-	|	-	|	(1,1)	|	Using CC License	|
5.2 Copyright	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|
5.3 Size	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|
5.4 URL - resource	|	-	|	ホームページ	|	-	|	url	|	Yes	|	URL	|	-	|	(1,1)	|	Request to provide us the data in the case that the data is published at differnt URL	|
5.5 Homepage URL	|	-	|	ホームページ【再掲】	|	-	|	url	|	-	|	-	|	-	|	-	|	-	|
5.6 Format - resource	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|
5.7 Language	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|


**Mappings to Other Vocabs**

Concept|CKAN - Level 1|CKAN - Level 2|CKAN - Level 3|Schema.org|DCAT|ADMS|VoID|Other (e.g. Dublin Core, Foaf, RDF, RDFa Lite)|RDFa Lite 1.1
------- | -------- | ----- | ---- | ---------- | ---------|-------|-------|-------|------
1 *Contact information*|||||||||
1.1 Person  | person | Yes | (1,1) | Contact person’s name for the asset.  |   Name should be formatted as Last, First
1.2 Contact Email  | mbox  | Yes | (1,1)  | Contact person’s email address.  |   Email address
1.3 Organisation (Owner) | publisher  | Yes |  (1,1) |  The publishing agency. |   Departments and multi-unit agencies may use this field to describe which subordinate agency published this dataset.
1.4 Publisher|-|-|-|-|-|-|-|-|-|
1.5 Author|-|-|-|-|-|-|-|-|-|
1.6 Author Email|-|-|-|-|-|-|-|-|-|
1.7 Maintainer|-|-|-|-|-|-|-|-|-|
1.8 Maintainer Email|-|-|-|-|-|-|-|-|-|
2 *Dataset information*|||||||||
2.1 Unique Identifier|identifier|-|-|-|-|-|-|-|-|
2.2 Release Date    | issued  | No  | (0,1)  | Date of formal issuance.  |    Date (YYYY-MM-DD)
2.3 Modified|-|-|-|-|-|-|-|-|-|
2.4 Last Updated  | modified  | Yes  | (1,1)  | Most recent date on which the dataset was changed, updated or modified.  |  Dates should be formatted as YYYY-MM-DD. Specify “01” as the day if unknown. 
2.5 Description | description | Yes | (1,1) | Human-readable description (e.g., an abstract) with sufficient detail to enable a user to quickly understand whether the asset is of interest. | string
2.6 Keyword | keyword  | Yes  | (1,n)  | Tags (or keywords) help users discover your dataset, please include terms that would be used by technical and non-technical users. |   Separate keywords with commas.
2.7 Frequency of Update  | accrualPeriodicity  |  No | (0,1)  |  Frequency with which dataset is published. |   Must be one of the following: hourly, daily, weekly, yearly, other
2.8 Title | title | Yes | (1,1) | Human-readable name of the asset. Should be in plain English and include sufficient detail to facilitate search and discovery. | string 
2.9 Category    | theme  |  No |  (0,n) |  Main thematic category of the dataset. |   Comma-separated values
GAP -|-|-|-|-|-|-|-|-|-|
3 *Extent information*|||||||||
3.1 Spatial Coverage | spatial  | If applicable  | (0,1)  | The range of spatial applicability of a dataset. Could include a spatial region like a bounding box or a named place.  |   This field should contain one of the following types of content: (1) a bounding coordinate box for the dataset represented in latitude / longitude pairs where the coordinates are specified in decimal degrees and in the order of: minimum longitude, minimum latitude, maximum longitude, maximum latitude; (2) a latitude / longitude pair (in decimal degrees) representing a point where the dataset is relevant; (3) a geographic feature expressed in Geography Markup Language using the Simple Features Profile; or (4) a geographic feature from the GeoNames database.
3.2 Spatial Type|-|-|-|-|-|-|-|-|-|
3.3 Spatial Coordinates|-|-|-|-|-|-|-|-|-|
3.4 Geographic Region Name|-|-|-|-|-|-|-|-|-|
3.5 Geographic Bounding Box - Lower Left Corner|-|-|-|-|-|-|-|-|-|
3.6 Bounding Box - Upper Right Corner|-|-|-|-|-|-|-|-|-|
3.7 Bounding Box - Coordinate Reference System|-|-|-|-|-|-|-|-|-|
3.8 Geographic Bounding Box - Dimensions|-|-|-|-|-|-|-|-|-|
3.9 Temporal Coverage | temporal   | If applicable  | (0,1)  |  The range of temporal applicability of a dataset (i.e., a start and end date of applicability for the data). |   This field should contain an interval of time defined by start and end dates. Dates should be formatted as pairs of {start date, end date} in the format YYYY-MM-DD hh:mm:ss using 24 hour clock time notation (e.g., 2011-02-14 12:00:00, 2013-02-14 12:00:00).
3.10 Temporal coverage starts|-|-|-|-|-|-|-|-|-|
3.11 Temporal coverage ends|-|-|-|-|-|-|-|-|-|
3.12 Temporal granularity|-|-|-|-|-|-|-|-|-|
3.13 Temporal granularity factor|-|-|-|-|-|-|-|-|-|
3.14 Periodicity of data collection|-|-|-|-|-|-|-|-|-|
3.15 Periodicity of the production process|-|-|-|-|-|-|-|-|-|
3.16 Periodicity of the estimates|-|-|-|-|-|-|-|-|-|
3.17 Temporal and spatial comparability|-|-|-|-|-|-|-|-|-|
3.18 Periodicity of data dissemination|-|-|-|-|-|-|-|-|-|
3.19 Data Quality    | dataQuality | No  | (0,1)  |  Whether the dataset meets the agency’s Information Quality Guidelines. | Boolean (true/false)    
3.20 Granularity    | granularity  | No  | (0,1)   | Level of granularity of the dataset.  |    Typically geographical or temporal.
4 *Supplemental information*|||||||||
4.1 Documentation | references  | No  | (0,n)  | Related documents such as technical information about a dataset, developer documentation, etc.  |   Comma-separated URLs
5 *Distribution information*|||||||||
5.1 License   | license  |  If applicable | (0,1)  | The license dataset or API is published with.  |   
5.2 Copyright|-|-|-|-|-|-|-|-|-|
5.3 Size    | size  | No  | (0,1)  | The size of the downloadable dataset.  |   Sizes should be formatted as (e.g.), 52kb, 140mb, 2gb.
5.4 Download URL | accessURL  | If applicable  |  (1,1) |  URL providing direct access to the downloadable distribution of a dataset. |   This must be the direct download URL. Use **landingPage** for landing or disambiguation pages, or **references** for documentation pages.
5.5 Homepage URL    |  landingPage |  No |(0,1) |  Alternative landing page used to redirect user to a contextual, Agency-hosted “homepage” for the Dataset or API when selecting this resource from the Data.gov user interface. |  URL; This field is not intended for an agency’s homepage (e.g. www.agency.gov), but rather if a dataset has a human-friendly hub or landing page that users should be directed to for all resources tied to the dataset. This allows agencies to better specify what a visitor receives after selecting one of the agency’s datasets on Data.gov or in third-party mashups.
5.6 Format (R)|The file format or API type of the distribution.|Format|format|res_format|If applicable|See Usage Notes|(0,1)|This must describe the exact file available at accessURL using file extensions (e.g., CSV, XLS, XSLX, TSV, JSON, XML). For example, if the download file is a ZIP containing a CSV, the entry here is “ZIP”.format|
5.7 Language (D)|The language of the dataset.|Language|language|-|No|string|^[a-z0-9_-]{2,}$|(0,n)|
US-specific Public Access Level  | accessLevel  | Yes  | (1,1) |  The degree to which this dataset could be made publicly-available, regardless of whether it has been made available. Choices: Public (is or could be made publicly available), Restricted (available under certain conditions), or Private (never able to be made publicly available)  |   Must be one of the following: Public, Restricted, Private
US-specific API Endpoint |  webService |  If applicable | (1,)  | Endpoint of web service to access dataset.  |   This field will serve to delineate the web services offered by an agency and will be used to aggregate cross-government API catalogs.
US-specific RSS Feed | feed | No | (0,1) | URL for an RSS feed that provides access to the dataset. | URL; These RSS feeds will be used to create a cross-agency RSS feed search tool.
US-specific Data Dictionary | dataDictionary  | If applicable  |(1,1) | URL to the data dictionary for the dataset or API. Note that documentation other than a Data Dictionary can be referenced using Related Documents as shown in the expanded fields.   |   URL
US-specific System of Records    | systemOfRecords  | No  | (0,1)  | URL to the System of Records related to this dataset.  |  URL

