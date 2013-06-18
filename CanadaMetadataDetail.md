####Canada Metadata

**Where to Find Data**

Where to find: [data.gc.ca](http://www.data.gc.ca)

Licensing: Open Government Licence - Canada

Contact: Mark Levene, Allanah Hilt

Latest metadata from: 30/05/2013

**Metadata Details**

Concept|Description|Front-end (human-readable)|National metadata schema|Back-end machine-readable|Required|Data Type|Format: pattern|Cardinality|Usage Notes
------- | -------- | ----- | ---- | ---------- | ---------|-------|-------|-------|------
1. *Contact information*  |	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|
1.1 Person		|	Contact person’s name for the asset.	|	Contact Name	|	person	|	maintainer	|	Yes	|	See Usage Notes	|	See Usage Notes	|	(1,1)	|	Name should be formatted as Last, First	|
1.2 Contact Email - Publisher	|	The electronic mail address of the responsible organization or individual	|	(=Email)	|	electronicMailAddress	|	author_email	|	YES	|	URL	|	-	|	(1,1)	|	-	|
1.2 Contact Email - Dataset	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|
1.3 Organisation (Owner)|	An entity responsible for making the resource available	|	Publisher	|	publisher 	|	owner_org	|	Yes	|	Text, based on encoding scheme	|	See Usage Notes	|	(1,1)	|	[Controlled Vocabulary - Government of Canada Registry of Applied Titles](http://www.tbs-sct.gc.ca/fip-pcim/reg-eng.asp)	|
1.4 Publisher	|	An entity responsible for making the resource available	|	Publisher	|	publisher 	|	owner_org	|	Yes	|	Text, based on encoding scheme	|	-	|	(1,1)	|[Controlled Vocabulary - Government of Canada Registry of Applied Titles](http://www.tbs-sct.gc.ca/fip-pcim/reg-eng.asp)|
1.5 Author|	An entity responsible for making the resource available	|	Publisher	|	publisher 	|	owner_org	|	Yes	|	Text, based on encoding scheme	|	-	|	(1,1)	|	[Controlled Vocabulary - Government of Canada Registry of Applied Titles](http://www.tbs-sct.gc.ca/fip-pcim/reg-eng.asp)|
1.6 Author Email|	The electronic mail address of the responsible organization or individual	|	(=Email)	|	electronicMailAddress	|	author_email	|	YES	|	URL	|	-	|	(1,1)	|	-	|
1.7 Maintainer	|	The electronic mail address of the responsible organization or individual	|	(=Email)	|	electronicMailAddress	|	author_email	|	YES	|	URL	|	-	|	(1,1)	|	-	|
1.8 Maintainer Email	|	The electronic mail address of the responsible organization or individual	|	(=Email)	|	electronicMailAddress	|	author_email	|	YES	|	URL	|	-	|	(1,1)	|	-	|
2. *Dataset Identification*	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|
2.1 Unique Identifier	|	A string which uniquely identifies the metadata file	|	File Identifier	|	fileIdentifier	|	id	|	Yes	|	See Usage Notes	|	Characters should be alphanumeric.	|	(1,1)	|	This field allows third parties to maintain a consistent record for datasets even if title or URLs are updated.	|
2.2 Release Date	|	Date of formal instance (e.g. publication) of the resource which includes the date when the resource is approvded for publication on the web. 	|	Date Published	|	issued	|	date_published	|	Yes	|	date	|	"YYYY-MM-DD See Usage Notes"	|	(1,1)	|[ISO 8601 Date and Time Formats - W3C](http://www.w3.org/TR/NOTE-datetime)	|
2.2.R Release Date|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|
2.3 Modified		|	The date in which the resource was modified	|	Date Modified	|	modified	|	modified	|	No	|	date	|	"YYYY-MM-DD See Usage Notes"	|	(0,1)	|	[ISO 8601 Date and Time Formats - W3C](http://www.w3.org/TR/NOTE-datetime)	|
2.3.R Modified	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|
2.4 Last Updated|	The date in which the resource was modified	|	Date Modified	|	modified	|	modified	|	If applicable	|	date	|	"YYYY-MM-DD See Usage Notes"	|	(0,1)	|	[ISO 8601 Date and Time Formats - W3C](http://www.w3.org/TR/NOTE-datetime)|
2.4.R Last Updated		|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|
2.5 Description	|	An account of the resource	|	Description	|	description	|	notes	|	Yes	|	string	|	^[a-z0-9_-]{2,}$	|	(1,1)	|	-	|
2.6 Keyword	|	Commonly used words or phrases which describe the resource.	|	Keywords  	|	keyword	|	keywords	|	Yes	|	Separate keywords with commas.	|	Separate keywords with commas.	|	(1,n)	|	Separate keywords with commas.	|
2.7 Frequency of Update	|	The frequency with which changes and additions are made to the resource after the initial resource is completed.	|	Frequency	|	maintainenceAndUpdateFrequency	|	maintenance_and_update_frequency	|	Yes	|	Text, based on encoding scheme	|	See Usage Notes	|	(1,1)	|	[Controlled vocabulary - North American Profile of ISO 19115:2003 : naoMD_MaintencanceFrequencyCode](http://nap.geogratis.gc.ca/metadata/register/registerItems-eng.html#RI_170)	|
2.8 Title	|	A name of a given (dataset)	|	Title	|	title	|	title	|	Yes	|	string	|	^[a-z0-9_-]{2,}$	|	(1,1)	|	-	|
2.9 Category	|	Theme	|	The topic of the resource	|	"Subject Topic Category"	|	subject	|	"subject topic_category"	|	Yes	|	Text, based on encoding scheme	|	See Usage Notes	|	(1,n)	|	[Controlled vocabulary: Government of Canada Core Subject Thesaurus](http://www.thesaurus.gc.ca/recherche-search/thes-eng.html)	|
3. *Extext*  |	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|
3.1 Spatial coverage	|Spatial characteristics of the resource	|	Spatial	|	spatial	|	spatial	|	If applicable	|	string	|	See Usage Notes	|	(0,1)	|	[Encoding scheme:The GeoJSON Format Specification](http://www.geojson.org/geojson-spec.html)	|
3.2 Spatial Type	|	The method used to spatially represent geographic information	|	Spatial Representation Type	|	spatialRepresentationType	|	spatial_representation_type	|	If applicable	|	Text, based on encoding scheme	|	See Usage Notes	|	-	|	-	|
3.3 Spatial Coordinates		|	Spatial characteristics of the resource	|	Spatial	|	spatial	|	spatial	|	If applicable	|	string	|	See Usage Notes	|	(0,1)	|	  [Encoding scheme:The GeoJSON Format Specification](http://www.geojson.org/geojson-spec.html)|
3.4 Geographic Region Name	|	The spatial or temporal topic of the resource, the spatial applicability of the resource, or the jurisdiction under which the resource is relevant.	|	Geographic Region	|	coverage	|	geographic_region	|	If applicable	|	Text, based on encoding scheme	|	See Usage Notes	|	(0,n)	|	[Controlled vocabulary :  Standard Geographical Classification (SGC)](http://www.statcan.gc.ca/subjects-sujets/standard-norme/sgc-cgt/2011/sgc-cgt-intro-eng.htm)	|
3.5 Geographic Bounding Box - Lower Left Corner  	|	Spatial characteristics of the resource	|	Spatial	|	spatial	|	spatial	|	If applicable	|	string	|	See Usage Notes	|	(0,1)	|	  [Encoding scheme:The GeoJSON Format Specification](http://www.geojson.org/geojson-spec.html)	|
3.6 Bounding Box - Upper Right Corner  	|	Spatial characteristics of the resource	|	Spatial	|	spatial	|	spatial	|	If applicable	|	string	|	See Usage Notes	|	(0,1)	|	  [Encoding scheme:The GeoJSON Format Specification](http://www.geojson.org/geojson-spec.html)	|
3.7 Bounding Box - Coordinate Reference System  |	Spatial characteristics of the resource	|	Spatial	|	spatial	|	spatial	|	If applicable	|	string	|	See Usage Notes	|	(0,1)	|  [Encoding scheme:The GeoJSON Format Specification](http://www.geojson.org/geojson-spec.html)	|
3.8 Geographic Bounding Box - Dimensions  |	Spatial characteristics of the resource	|	Spatial	|	spatial	|	spatial	|	If applicable	|	string	|	See Usage Notes	|	(0,1)	|	  [Encoding scheme:The GeoJSON Format Specification](http://www.geojson.org/geojson-spec.html)	|
3.9 Temporal coverage	|	Temporal characteristics of a resource. 	|	(=Temporal)	|	timePeriodCoverageStart/timePeriodCoverageEnd	|	time_period_coverage_start/time_period_coverage_end	|	If applicable	|	date	|	"YYYY-MM-DD See Usage Notes"	|	(0,1)	|	ISO 8601 Date and Time Formats - W3C	|
3.10 Temporal coverage starts	|	Temporal characteristics of a resource. The start date or time interval (s) convered by the data.	|	Time Period Coverage Start  	|	timePeriodCoverageStart	|	time_period_coverage_start	|	If applicable	|	date	|	"YYYY-MM-DD See Usage Notes"	|	(0,1)	|	[ISO 8601 Date and Time Formats - W3C](http://www.w3.org/TR/NOTE-datetime)  	|
3.11 Temporal coverage ends	|	Temporal characteristics of a resource. The end date or time intervals (s) covered by the data.	|	Time Period Coverage End	|	timePeriodCoverageEnd	|	time_period_coverage_end	|	If applicable	|	date	|	"YYYY-MM-DD See Usage Notes"	|	(0,1)	|[ISO 8601 Date and Time Formats - W3C](http://www.w3.org/TR/NOTE-datetime)  	|
3.12 Temporal granularity	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|
3.13 Temporal granularity factor	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|
3.14 Periodicity of data(set) collection	|	The frequency with which changes and additions are made to the resource after the initial resource is completed.	|	Frequency	|	maintainenceAndUpdateFrequency	|	maintenance_and_update_frequency	|	Yes	|	Text, based on encoding scheme	|	See Usage Notes	|	(1,1)	|	[Controlled vocabulary - North American Profile of ISO 19115:2003 : naoMD_MaintencanceFrequencyCode](http://nap.geogratis.gc.ca/metadata/register/registerItems-eng.html#RI_170)	|
3.15 Periodicity of the production process	|	The frequency with which changes and additions are made to the resource after the initial resource is completed.	|	Frequency	|	maintainenceAndUpdateFrequency	|	maintenance_and_update_frequency	|	Yes	|	Text, based on encoding scheme	|	See Usage Notes	|	(1,1)	|	[Controlled vocabulary - North American Profile of ISO 19115:2003 : naoMD_MaintencanceFrequencyCode](http://nap.geogratis.gc.ca/metadata/register/registerItems-eng.html#RI_170)	|
3.16 Periodicity of the estimates	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|
3.17 Temporal and spatial comparability	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|
3.18 Periodicity of data dissemination		|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|
3.19 Data quality	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|
3.20 Reference period	|	Temporal characteristics of a resource. 	|	(=Temporal)	|	timePeriodCoverageStart/timePeriodCoverageEnd	|	time_period_coverage_start/time_period_coverage_end	|	If applicable	|	date	|	"YYYY-MM-DD See Usage Notes"	|	(0,1)	|	[ISO 8601 Date and Time Formats - W3C](http://www.w3.org/TR/NOTE-datetime)  	|
4. *Supplemental Information*	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|
4.1 Documentation URL - resource	|	The type of resource	|	Resource Type	|	resourceType	|	resource_type	|	Yes	|	Text, based on encoding scheme	|	See Usage Notes	|	(1,1)	|	Controlled list	|
5. *Distribution information*	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|
5.1 Licence	|	The limitations or constraints on the use of the resource	|	Licence	|	useConstraints	|	licence_id	|	Yes	|	string	|	-	|	(1,1)	|	-	|
5.2 Copyright	|	The limitations or constraints on the use of the resource	|	(=Licence)	|	useConstraints	|	licence_id	|	Yes	|	string	|	-	|	(1,1)	|	-	|
5.3 Size		|	The estimated size of a unit in the specified transfer format.	|	Size	|	transferSize	|	size	|	Yes	|	numeric	|	Expressed in Bytes	|	(1,1)	|	-	|
5.4 URL - resource		|	The location (address) for on-line access using a Unifrom Resource Locator address or similar addressing scheme.	|	URL	|	linkage	|	url	|	Yes	|	string	|	-	|	(1,1)	|	-	|
5.5 Homepage URL		|	The URL for the Government of Canada program that is responsible for the dataset.	|	Homepage URL	|	homepageUrl	|	url	|	If applicable	|	URL	|	-	|	(0,1)	|	-	|
5.6 Format - resource		|	The name of the data transfer format.	|	Format	|	name	|	format	|	YES	|	Text, based on encoding scheme	|	See Usage Notes	|	(1,1)	|	Controlled list.	|
5.7 Language	|	The language of the resource	|	Language	|	language	|	language	|	Yes	|	Text, based on encoding scheme	|	See Usage Notes	|	(1,1)	|	Controlled vocabulary : Codes for the Representation of Names of Language, Part 2: Alpha-3 Code / Terminology Codes (ISO 639-2/T) and ISO 3166-1 country codes	|


**Mappings to Other Vocabs**

Concept | Human-Readable Label | Metadata | CKAN | RDFa Lite 1.1 | Schema.org
------- | ----- | -------- | -------- | -------- | ----- | -------

