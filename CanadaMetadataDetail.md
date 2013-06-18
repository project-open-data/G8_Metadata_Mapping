####Canada Metadata

**Where to Find Data**

Where to find: [data.gc.ca](http://www.data.gc.ca)
Licensing: Open Government Licence - Canada
Contact: Mark Levene, Allanah Hilt
Latest metadata from: 30/05/2013

**Metadata Details**

Concept | Metadata | Required? | Cardinality | Description | Usage Notes
------- | -------- | ----- | ---- | ---------- | ---------
1. Contact information  |	Concept	|	Description	|	Front-end label	|	National metadata schema term	|	Back-end label	|	Required?	|	Data type	|	Format: pattern	|	Cardinality	|	Usage notes	|
1.1 Person	|	Person (individual who fulfils either one or more of the following roles in relation to the data(set): creator; owner; maintainer; publisher; editor; contact)	|	Contact person’s name for the asset.	|	Contact Name	|	person	|	maintainer	|	Yes	|	See Usage Notes	|	See Usage Notes	|	(1,1)	|	Name should be formatted as Last, First	|
1.2 Contact Email - Publisher	|	Contact Email (associated with Publisher - might be individual, office or institution)	|	The electronic mail address of the responsible organization or individual	|	(=Email)	|	electronicMailAddress	|	author_email	|	YES	|	URL	|	-	|	(1,1)	|	-	|
1.2 Contact Email - Dataset	|	Contact Email (associated with dataset - might be individual, office or institution; this is common just the email associated with the Publisher)	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|
1.3 Organisation (Owner)	|	Organisation (institution who fulfils one or more of the following roles with respect to the data: creator; owner; maintainer; publisher; editor; contact)	|	An entity responsible for making the resource available	|	Publisher	|	publisher 	|	owner_org	|	Yes	|	Text, based on encoding scheme	|	See Usage Notes	|	(1,1)	|	Controlled Vocabulary - Government of Canada Registry of Applied Titles	|
1.4 Publisher	|	Publisher (individual, office or institution who publishes the data(set))	|	An entity responsible for making the resource available	|	Publisher	|	publisher 	|	owner_org	|	Yes	|	Text, based on encoding scheme	|	-	|	(1,1)	|	Controlled Vocabulary - Government of Canada Registry of Applied Titles	|
1.5 Author	|	Author (individual, office or institution who fulfils one or more of the following roles in relation to the data: owner; publisher; editor; creator; contact)	|	An entity responsible for making the resource available	|	Publisher	|	publisher 	|	owner_org	|	Yes	|	Text, based on encoding scheme	|	-	|	(1,1)	|	Controlled Vocabulary - Government of Canada Registry of Applied Titles	|
1.6 Author Email	|	Author Email (email address of author)	|	The electronic mail address of the responsible organization or individual	|	(=Email)	|	electronicMailAddress	|	author_email	|	YES	|	URL	|	-	|	(1,1)	|	-	|
1.7 Maintainer	|	Maintainer (individual, office or institution who maintains the dataset, i.e. Ensures it continues to be available and who may also be the main contact)	|	The electronic mail address of the responsible organization or individual	|	(=Email)	|	electronicMailAddress	|	author_email	|	YES	|	URL	|	-	|	(1,1)	|	-	|
1.8 Maintainer Email	|	Maintainer Email (email address of maintainer)	|	The electronic mail address of the responsible organization or individual	|	(=Email)	|	electronicMailAddress	|	author_email	|	YES	|	URL	|	-	|	(1,1)	|	-	|
2. Dataset Identification	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|
2.1 Unique Identifier	|	Unique identifier (string that uniquely references dataset or resource within its portal)	|	A string which uniquely identifies the metadata file	|	File Identifier	|	fileIdentifier	|	id	|	Yes	|	See Usage Notes	|	Characters should be alphanumeric.	|	(1,1)	|	This field allows third parties to maintain a consistent record for datasets even if title or URLs are updated.	|
2.2 Release Date	|	Release date (date that dataset published at URL)	|	Date of formal instance (e.g. publication) of the resource which includes the date when the resource is approvded for publication on the web. 	|	Date Published	|	issued	|	date_published	|	Yes	|	date	|	"YYYY-MM-DD
See Usage Notes"	|	(1,1)	|	ISO 8601 Date and Time Formats - W3C	|
2.2.R Release Date	|	Release date (date that resource published at URL)	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|
2.3 Modified	|	Modified (date that this dataset was changed)	|	The date in which the resource was modified	|	Date Modified	|	modified	|	modified	|	No	|	date	|	"YYYY-MM-DD
See Usage Notes"	|	(0,1)	|	ISO 8601 Date and Time Formats - W3C	|
2.3.R Modified	|	Modified (date that this resource was changed)	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|
2.4 Last Updated	|	Last updated (date that this dataset was changed)	|	The date in which the resource was modified	|	Date Modified	|	modified	|	modified	|	If applicable	|	date	|	"YYYY-MM-DD
See Usage Notes"	|	(0,1)	|	ISO 8601 Date and Time Formats - W3C	|
2.4.R Last Updated	|	Last updated (date that this resource was changed)	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|
2.5 Description	|	Description (textual description of a dataset)	|	An account of the resource	|	Description	|	description	|	notes	|	Yes	|	string	|	^[a-z0-9_-]{2,}$	|	(1,1)	|	-	|
2.6 Keyword	|	Keyword (free-text words that help people discover a given dataset)	|	Commonly used words or phrases which describe the resource.	|	Keywords  	|	keyword	|	keywords	|	Yes	|	Separate keywords with commas.	|	Separate keywords with commas.	|	(1,n)	|	Separate keywords with commas.	|
2.7 Frequency of Update	|	Frequency of update (indication of how often a dataset are updated)	|	The frequency with which changes and additions are made to the resource after the initial resource is completed.	|	Frequency	|	maintainenceAndUpdateFrequency	|	maintenance_and_update_frequency	|	Yes	|	Text, based on encoding scheme	|	See Usage Notes	|	(1,1)	|	Controlled vocabulary - North American Profile of ISO 19115:2003 : naoMD_MaintencanceFrequencyCode	|
2.8 Title	|	Title (Short textual name which briefly describes a dataset)	|	A name of a given (dataset)	|	Title	|	title	|	title	|	Yes	|	string	|	^[a-z0-9_-]{2,}$	|	(1,1)	|	-	|
2.9 Category	|	Theme	|	The topic of the resource	|	"Subject 
Topic Category"	|	subject	|	"subject
topic_category"	|	Yes	|	Text, based on encoding scheme	|	See Usage Notes	|	(1,n)	|	Controlled vocabulary: Government of Canada Core Subject Thesaurus	|
3.1 Spatial coverage	|	Spatial coverage (dataset)	|	Spatial characteristics of the resource	|	Spatial	|	spatial	|	spatial	|	If applicable	|	string	|	See Usage Notes	|	(0,1)	|	Encoding scheme:The GeoJSON Format Specification	|
3.2 Spatial Type	|	Spatial type	|	The method used to spatially represent geographic information	|	Spatial Representation Type	|	spatialRepresentationType	|	spatial_representation_type	|	If applicable	|	Text, based on encoding scheme	|	See Usage Notes	|	-	|	-	|
3.3 Spatial Coordinates	|	Spatial coordinates	|	Spatial characteristics of the resource	|	Spatial	|	spatial	|	spatial	|	If applicable	|	string	|	See Usage Notes	|	(0,1)	|	Encoding scheme:The GeoJSON Format Specification	|
3.4 Geographic Region Name	|	Geographic Region Name	|	The spatial or temporal topic of the resource, the spatial applicability of the resource, or the jurisdiction under which the resource is relevant.	|	Geographic Region	|	coverage	|	geographic_region	|	If applicable	|	Text, based on encoding scheme	|	See Usage Notes	|	(0,n)	|	Controlled vocabulary :  Standard Geographical Classification (SGC)	|
3.5 Geographic Bounding Box - Lower Left Corner  	|	Geographic Bounding Box - Lower Left Corner  	|	Spatial characteristics of the resource	|	Spatial	|	spatial	|	spatial	|	If applicable	|	string	|	See Usage Notes	|	(0,1)	|	Encoding scheme:The GeoJSON Format Specification	|
3.6 Bounding Box - Upper Right Corner  	|	Bounding Box - Upper Right Corner  	|	Spatial characteristics of the resource	|	Spatial	|	spatial	|	spatial	|	If applicable	|	string	|	See Usage Notes	|	(0,1)	|	Encoding scheme:The GeoJSON Format Specification	|
3.7 Bounding Box - Coordinate Reference System  	|	Bounding Box - Coordinate Reference System  	|	Spatial characteristics of the resource	|	Spatial	|	spatial	|	spatial	|	If applicable	|	string	|	See Usage Notes	|	(0,1)	|	Encoding scheme:The GeoJSON Format Specification	|
3.8 Geographic Bounding Box - Dimensions  	|	Geographic Bounding Box - Dimensions  	|	Spatial characteristics of the resource	|	Spatial	|	spatial	|	spatial	|	If applicable	|	string	|	See Usage Notes	|	(0,1)	|	Encoding scheme:The GeoJSON Format Specification	|
3.9 Temporal coverage	|	Temporal coverage	|	Temporal characteristics of a resource. 	|	(=Temporal)	|	timePeriodCoverageStart/timePeriodCoverageEnd	|	time_period_coverage_start/time_period_coverage_end	|	If applicable	|	date	|	"YYYY-MM-DD
See Usage Notes"	|	(0,1)	|	ISO 8601 Date and Time Formats - W3C	|
3.10 Temporal coverage starts	|	Temporal coverage starts (dataset)	|	Temporal characteristics of a resource. The start date or time interval (s) convered by the data.	|	Time Period Coverage Start  	|	timePeriodCoverageStart	|	time_period_coverage_start	|	If applicable	|	date	|	"YYYY-MM-DD
See Usage Notes"	|	(0,1)	|	ISO 8601 Date and Time Formats - W3C	|
3.11 Temporal coverage ends	|	Temporal coverage ends	|	Temporal characteristics of a resource. The end date or time intervals (s) covered by the data.	|	Time Period Coverage End	|	timePeriodCoverageEnd	|	time_period_coverage_end	|	If applicable	|	date	|	"YYYY-MM-DD
See Usage Notes"	|	(0,1)	|	ISO 8601 Date and Time Formats - W3C	|
3.12 Temporal granularity	|	Temporal granularity (dataset)	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|
3.13 Temporal granularity factor	|	Temporal granularity factor	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|
3.14 Periodicity of data(set) collection	|	Periodicity of data(set) collection	|	The frequency with which changes and additions are made to the resource after the initial resource is completed.	|	Frequency	|	maintainenceAndUpdateFrequency	|	maintenance_and_update_frequency	|	Yes	|	Text, based on encoding scheme	|	See Usage Notes	|	(1,1)	|	Controlled vocabulary - North American Profile of ISO 19115:2003 : naoMD_MaintencanceFrequencyCode	|
3.15 Periodicity of the production process	|	Periodicity of the production process	|	The frequency with which changes and additions are made to the resource after the initial resource is completed.	|	Frequency	|	maintainenceAndUpdateFrequency	|	maintenance_and_update_frequency	|	Yes	|	Text, based on encoding scheme	|	See Usage Notes	|	(1,1)	|	Controlled vocabulary - North American Profile of ISO 19115:2003 : naoMD_MaintencanceFrequencyCode	|
3.16 Periodicity of the estimates	|	Periodicity of the estimates	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|
3.17 Temporal and spatial comparability	|	Temporal and spatial comparability	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|
3.18 Periodicity of data dissemination	|	Periodicity of data dissemination	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|
3.19 Data quality	|	Data quality	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|
3.20.X Reference period	|	Reference period	|	Temporal characteristics of a resource. 	|	(=Temporal)	|	timePeriodCoverageStart/timePeriodCoverageEnd	|	time_period_coverage_start/time_period_coverage_end	|	If applicable	|	date	|	"YYYY-MM-DD
See Usage Notes"	|	(0,1)	|	ISO 8601 Date and Time Formats - W3C	|
4. Supplemental Information	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|
4.1 Documentation URL - resource	|	Documentation URL (resource)	|	The type of resource	|	Resource Type	|	resourceType	|	resource_type	|	Yes	|	Text, based on encoding scheme	|	See Usage Notes	|	(1,1)	|	Controlled list	|
-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|
5.1 Licence	|	Licence (dataset)	|	The limitations or constraints on the use of the resource	|	Licence	|	useConstraints	|	licence_id	|	Yes	|	string	|	-	|	(1,1)	|	-	|
5.2 Copyright	|	Copyright	|	The limitations or constraints on the use of the resource	|	(=Licence)	|	useConstraints	|	licence_id	|	Yes	|	string	|	-	|	(1,1)	|	-	|
5.3 Size	|	Size (dataset)	|	The estimated size of a unit in the specified transfer format.	|	Size	|	transferSize	|	size	|	Yes	|	numeric	|	Expressed in Bytes	|	(1,1)	|	-	|
5.4 URL - resource	|	URL (resource)	|	The location (address) for on-line access using a Unifrom Resource Locator address or similar addressing scheme.	|	URL	|	linkage	|	url	|	Yes	|	string	|	-	|	(1,1)	|	-	|
5.5 Homepage URL	|	Homepage	|	The URL for the Government of Canada program that is responsible for the dataset.	|	Homepage URL	|	homepageUrl	|	url	|	If applicable	|	URL	|	-	|	(0,1)	|	-	|
5.6 Format - resource	|	Format (resource)	|	The name of the data transfer format.	|	Format	|	name	|	format	|	YES	|	Text, based on encoding scheme	|	See Usage Notes	|	(1,1)	|	Controlled list.	|
5.7 Language	|	Language (dataset)	|	The language of the resource	|	Language	|	language	|	language	|	Yes	|	Text, based on encoding scheme	|	See Usage Notes	|	(1,1)	|	Controlled vocabulary : Codes for the Representation of Names of Language, Part 2: Alpha-3 Code / Terminology Codes (ISO 639-2/T) and ISO 3166-1 country codes	|


**Mappings to Other Vocabs**

Concept | Human-Readable Label | Metadata | CKAN | RDFa Lite 1.1 | Schema.org
------- | ----- | -------- | -------- | -------- | ----- | -------

