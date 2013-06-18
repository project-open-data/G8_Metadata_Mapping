####France Metadata

**Where to Find Data**

Where to find: Data of the EU institutions are hosted with the different institutions and departments. The open data portal of the EU institutions references metadata to datasets selected for this portal.

Licensing: [Click here](http://ec.europa.eu/geninfo/legal_notices_en.htm)

Contact: op-odp-contact@publications.europa.eu

Latest metadata: http://open-data.europa.eu/files/MetadataVocabulary.ods

**Metadata Details**

Concept|Description|Front-end (human-readable)|National metadata schema|Back-end machine-readable|Required|Data Type|Format: pattern|Cardinality|Usage Notes
------- | -------- | ----- | ---- | ---------- | ---------|-------|-------|-------|------
1. *Contact information*  |  -  |	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|
1.1 Person  |	Name of the contact (person or role)	|	Ansprechpartner	|	-	|	extras->contacts->name	|	yes	|	String	|	-	|	(1,2)	|	As "extras->contacts" is a list, it is possible to define a "publisher" and an "author" (--> "extras->contacts->role")	|
1.2 Contact Email - Publisher	|	Email address of contact.	|	Ansprechpartner: E-Mail	|	-	|	extras->contacts->email	|	no	|	String	|	-	|	(0,2)	|	see "person"	|
1.2 Contact Email - Dataset	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|
1.3 Organisation (Owner)	|	-	|	(= Maintainer OR author)	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|
1.4 Publisher	|	-	|	(= Author)	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|
1.5 Author	|	The authority from which the data originated.	|	Veröffentlichende Stelle	|	-	|	author	|	yes	|	String	|	-	|	(1,1)	|	-	|
1.6 Author Email	|	Email address or contact form of the author.	|	Veröffentlichende Stelle: E-Mail	|	-	|	author_email	|	no	|	String	|	URI	|	(0,1)	|	Instead of an email address, it is possible to include the URL of a web-based contact form.	|
1.7 Maintainer	|	This contact (normally an authority or role, not an individual) should be contacted for questions and comments on the data.	|	Datenverantwortliche Stelle	|	-	|	maintainer	|	no	|	String	|	-	|	(0,1)	|	-	|
1.8 Maintainer Email	|	Email address or contact form of responsible authority.	|	Datenverantwortliche Stelle: E-Mail	|	-	|	maintainer_email	|	no	|	String	|	URI	|	(0,1)	|	Instead of an email address, it is possible to include the URL of a web-based contact form.	|
2. Dataset Identification	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|
2.1 Unique Identifier	|	A human readable identifier that can be used for identification (ASCII-version of "title", used for "pretty links" and linked data URIs)	|	Name	|	-	|	name	|	yes	|	String	|	^[a-z0-9_-]{2,}$	|	(1,1)	|	-	|
2.2 Release Date	|	Publication data of the dataset.	|	Veröffentlichungsdatum	|	-	|	 (extras->dates->role = "veroeffentlicht"): extras->dates->date	|	yes	|	String	|	date (DD.MM.YYYY)	|	(1,1)	|	"extras->dates" is a list, containing the dates of creation, publicaton and last modification of the dataset. To include the release date, "extras->dates->role" has to be set to "veroeffentlicht".	|
2.2.R Release Date	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|
2.3 Modified	|	Date that this dataset or the metadata was changed.	|	Stand Metadaten 	|	-	|	(extras->dates->role = "aktualisiert") extras->dates->date	|	yes	|	string	|	date (DD.MM.YYYY)	|	(1,1)	|	"extras->dates" is a list, containing the dates of creation, publicaton and last modification of the dataset. To include the release date, "extras->dates->role" has to be set to "aktualisiert".	|
2.3.R Modified	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|
2.4 Last Updated	|	-	|	[= Modified (date that this dataset was changed)]	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|
2.4.R Last Updated	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|
2.5 Description	|	Human readable description and additional information.	|	Beschreibung	|	-	|	notes	|	yes	|	String	|	-	|	(1,1)	|	-	|
2.6 Keyword	|	Free-text keywords (or tags)	|	Schlagwörter	|	-	|	tags	|	no	|	List of strings	|	-	|	(0,n)	|	-	|
2.7 Frequency of Update	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|
2.8 Title	|	The title describes the dataset and is displayed for example in search results and lists.	|	Titel	|	-	|	title	|	yes	|	String	|	-	|	(1,1)	|	-	|
2.9 Category	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|
3. Extent	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|
3.1 Spatial coverage	|	The geographical coverage of the data.	|	Geographische Abdeckung	|	-	|	(see below)	|	-	|	-	|	-	|	-	|	Currently not used by GovData. Will be used later for geographical search.	|
3.2 Spatial Type	|	At the moment, just a polygon is provided, other types could be envisaged in future.	|	Art der Form	|	-	|	extras->spatial->type	|	no	|	String	|	Chose from "polygon"	|	(0,1)	|	Currently, "polygon" is the sole list element	|
3.3 Spatial Coordinates	|	List of the coordinates	|	Koordinaten-Liste	|	-	|	extras->spatial->coordinates	|	no	|	List of arrays	|	-	|	(0,n)	|	WGS 84 coordinates according to GeoJSON (http://geojson.org)	|
3.4 Geographic Region Name	|	Covered area, if possible, the Official location key. Will be used later for a geographic search.	|	Abgedecktes Gebiet	|	-	|	extras->spatial_text	|	no	|	String	|	-	|	(0,1)	|	Currently not used by GovData. Will be used later for geographical search.	|
3.5 Geographic Bounding Box - Lower Left Corner  	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|
3.6 Bounding Box - Upper Right Corner  	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|
3.7 Bounding Box - Coordinate Reference System  	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|
3.8 Geographic Bounding Box - Dimensions  	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|
3.9 Temporal coverage	|	-	|	Zeitliche Abdeckung	|	-	|	(see below)	|	-	|	-	|	-	|	-	|	-	|
3.10 Temporal coverage starts	|	The start time-related endpoint of the dataset.	|	Zeitliche Abdeckung: Start-Datum	|	-	|	extras->temporal_coverage_from	|	no	|	String	|	date (DD.MM.YYYY)	|	(0,1)	|	-	|
3.11 Temporal coverage ends	|	The final time-related endpoint of the dataset.	|	Zeitliche Abdeckung: End-Datum	|	-	|	extras->temporal_coverage_to	|	no	|	String	|	date (DD.MM.YYYY)	|	(0,1)	|	-	|
3.12 Temporal granularity	|	The temporal granularity of the data.	|	Zeitliche Auflösung	|	-	|	extras->temporal_granularity	|	no	|	String	|	Choose from second, minute, hour, day, week, month, quarter, year, 5-year	|	(0,1)	|	-	|
3.13 Temporal granularity factor	|	With this factor, the temporal resolution can be set to "n times temporal_granularity".	|	Faktor für die zeitliche Auflösung	|	-	|	extras->temporal_granularity_factor	|	-	|	Number	|	-	|	-	|	e.g. "15 minutes"	|
3.14 Periodicity of data(set) collection	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|
3.15 Periodicity of the production process	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|
3.16 Periodicity of the estimates	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|
3.17 Temporal and spatial comparability	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|
3.18 Periodicity of data dissemination	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|
3.19 Data quality	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|
3.20.X Reference period	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|
4. Supplemental Information	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|
4.1 Documentation URL - resource	|	The original website the data is coming from.	|	Website	|	-	|	url	|	no	|	string	|	URI	|	(0,1)	|	-	|
5. Supplemental Information	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|
5.1 Licence	|	-	|	Nutzungsbestimmungen	|	-	|	license_id	|	yes	|	string	|	Choose from apache, app_commercial, app_freeware, app_opensource, bsd-license, cc-by, cc-by-sa, cc-nc, cc-by-nd, cc-zero, dl-de-by-1.0, dl-de-by-nc-1.0, geolizenz-closed, geolizenz-i-a, gfdl, gpl-3.0, mozilla, odc-by, odc-odbl, odc-pddl, official-work, other-closed, other-open	|	(1,1)	|	-	|
5.2 Copyright	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|
5.3 Size	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|
5.4 URL - resource	|	The URL of the resource	|	Link	|	-	|	resources->url	|	yes	|	String	|	URI	|	(1,n)	|	As "resources" is a list of objects, more than one resource (each including one URL) may be defined.	|
5.5 Homepage URL	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|
5.6 Format - resource	|	Type of resource	|	Format	|	-	|	resources->format	|	yes	|	String	|	-	|	(1,n)	|	MIME type.
As "resources" is a list of objects, more than one resource (each including one format / type) may be defined.|
5.7 Language	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	The language can be defined only per resource, not per dataset!	|





**Mappings to Other Vocabs**

Concept | Human-Readable Label | Metadata | CKAN | RDFa Lite 1.1 | Schema.org
------- | ----- | -------- | -------- | -------- | ----- | -------

