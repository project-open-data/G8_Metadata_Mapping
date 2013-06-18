####EU Metadata

**Where to Find Data**

Where to find: Data of the EU institutions are hosted with the different institutions and departments. The open data portal of the EU institutions references metadata to datasets selected for this portal.

Licensing: [Click here](http://ec.europa.eu/geninfo/legal_notices_en.htm)

Contact: op-odp-contact@publications.europa.eu

Latest metadata: http://open-data.europa.eu/files/MetadataVocabulary.ods

**Metadata Details**

Concept|Description|Front-end (human-readable)|National metadata schema|Back-end machine-readable|Required|Data Type|Format: pattern|Cardinality|Usage Notes
------- | -------- | ----- | ---- | ---------- | ---------|-------|-------|-------|------
1. *Contact information*  |  -	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|
1.1 Person	|	The name of the main contact for enquiries about the dataset	|	Contact Name	|	-	|	contact_name	|	-	|	RDF literal	|	-	|	(1,1)	|	-	|
1.2 Contact Email - Publisher	|	-	|	Contact / Email	|	-	|	contact_email	|	-	|	RDF literal	|	-	|	(0,1)	|	-	|
1.2 Contact Email - Dataset	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|
1.3 Organisation (Owner)	|	-	|	Contact Point	|	-	|	-	|	-	|	Resource	|	-	|	(0,1))	|	-	|
1.4 Publisher	|	-	|	Publisher	|	-	|	published_by	|	-	|	NAL code	|	-	|	(1,1)	|	-	|
1.5 Author	|	-	|	Contact Name	|	-	|	contact_name	|	-	|	RDF literal	|	-	|	(1,1)	|	-	|
1.6 Author Email	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|
1.7 Maintainer	|	-	|	Contact Name	|	-	|	contact_name	|	-	|	RDF literal	|	-	|	(1,1)	|	-	|
1.8 Maintainer Email	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|
2. *Dataset Identification*	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|
2.1 Unique Identifier	|	Uniform resource identifier	|	URI	|	-	|	-	|	-	|	RDF literal	|	-	|	(1,1)	|	-	|
2.2 Release Date	|	Date of formal issuance (e.g. publication) o fthe dataset	|	Issued	|	-	|	release_date	|	-	|	Datetime	|	-	|	(0,1)	|	-	|
2.2.R Release Date	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|
2.3 Modified	|	Most recent date on which the dataset was changed, updated or modified	|	Modified date	|	-	|	modified_date	|	-	|	Datetime	|	-	|	(1,1)	|	-	|
2.3.R Modified	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|
2.4 Last Updated	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|
2.4.R Last Updated	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|
2.5 Description	|	Description	|	Description	|	-	|	description	|	-	|	RDF literal	|	-	|	-	|	-	|
2.6 Keyword	|	-	|	Keyword	|	-	|	keyword_string	|	-	|	RDF literal	|	-	|	-	|	-	|
2.7 Frequency of Update	|	The frequency with which the dataset is published	|	accrual periodicity	|	-	|	update_frequency	|	-	|	RDF literal	|	-	|	(0,1)	|	-	|
2.8 Title	|	-	|	Title	|	-	|	title	|	-	|	RDF literal	|	-	|	(1,1)	|	-	|
2.9 Category	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|
3 *Extent*	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|
3.1 Spatial coverage	|	-	|	Geographical coverage	|	-	|	geographical_coverage	|	-	|	NAL code	|	-	|	-	|	-	|
3.2 Spatial Type	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|
3.3 Spatial Coordinates	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|
3.4 Geographic Region Name	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|
3.5 Geographic Bounding Box - Lower Left Corner  	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|
3.6 Bounding Box - Upper Right Corner  	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|
3.7 Bounding Box - Coordinate Reference System  	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|
3.8 Geographic Bounding Box - Dimensions  	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|
3.9 Temporal coverage	|	-	|	Temporal coverage	|	-	|	-	|	-	|	Resource	|	-	|	(0,1)	|	-	|
3.10 Temporal coverage starts	|	-	|	Temporal coverage from	|	-	|	temporal_coverage_from	|	-	|	Datetime	|	-	|	(0,1)	|	-	|
3.11 Temporal coverage ends	|	-	|	Temporal coverage to	|	-	|	temporal_coverage_to	|	-	|	Datetime	|	-	|	(0,1)	|	-	|
3.12 Temporal granularity	|	-	|	temporal coverage / granularity	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|
3.13 Temporal granularity factor	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|
3.14 Periodicity of data(set) collection	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|
3.15 Periodicity of the production process	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|
3.16 Periodicity of the estimates	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|
3.17 Temporal and spatial comparability	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|
3.18 Periodicity of data dissemination	|	-	|	acrrual periodicity	|	-	|	accural_periodicity	|	-	|	RDF literal	|	-	|	(0,1)	|	-	|
3.19 Data quality	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|
3.20.X Reference period	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|
4. *Supplemental Information*	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|
4.1 Documentation URL - resource	|	-	|	Documentation / URL	|	-	|	url	|	-	|	URL	|	-	|	(1,1)	|	-	|
5. *Distribution Information*	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|
5.1 Licence	|	-	|	Licence	|	-	|	license_id	|	-	|	NAL code	|	-	|	-	|	-	|
5.2 Copyright	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|
5.3 Size	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|
5.4 URL - resource	|	-	|	Distribution/URL	|	-	|	url	|	-	|	URL	|	-	|	(1,1)	|	-	|
5.5 Homepage URL	|	-	|	URL/HOME	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|
5.6 Format - resource	|	-	|	Distribution/Format	|	-	|	format	|	-	|	RDF literal	|	-	|	(1,1)	|	-	|
5.7 Language	|	-	|	language	|	-	|	language	|	-	|	NAL code	|	-	|	-	|	-	|



**Mappings to Other Vocabs**

Concept|CKAN - Level 1|CKAN - Level 2|CKAN - Level 3|Schema.org|DCAT|ADMS|VoID|Other (e.g. Dublin Core, Foaf, RDF, RDFa Lite)|
------- | -------- | ----- | ---- | ---------- | ---------|-------|-------|-------|------
1. Contact information  |	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|
1.1 Person	|	extra:contact_name	|	-	|	-	|	sdo:Person	|	foaf:Person	|	-	|	-	|	-	|
1.2 Contact Email - Publisher	|	extra:contact_email	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|
1.2 Contact Email - Dataset	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|
1.3 Organisation (Owner)	|	-	|	-	|	-	|	sdo:Organization	|	foaf:Organization	|	-	|	-	|	-	|
1.4 Publisher	|	group:publisher	|	-	|	-	|	sdo:publisher	|	dcterms:publisher	|	dcterms:publisher	|	-	|	-	|
1.5 Author	|	extra:contact_name	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|
1.6 Author Email	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|
1.7 Maintainer	|	extra:contact_name	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|
1.8 Maintainer Email	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|
2. Dataset Identification	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|
2.1 Unique Identifier	|	dataset:id	|	-	|	-	|	-	|	dcterms:identifier	|	-	|	-	|	-	|
2.2 Release Date	|	extra:release_date	|	-	|	-	|	sdo:datePublished	|	dcterms:issued	|	dcterms:created	|	-	|	-	|
2.2.R Release Date	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|
2.3 Modified	|	extra:modified_date	|	-	|	-	|	sdo:dateModified	|	dcterms:modified	|	dcterms:modified	|	-	|	-	|
2.3.R Modified	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|
2.4 Last Updated	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|
2.4.R Last Updated	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|
2.5 Description	|	dataset:notes	|	-	|	-	|	sdo:description	|	dcterms:description	|	dcterms:description	|	-	|	-	|
2.6 Keyword	|	dataset:tags	|	-	|	-	|	sdo:keywords	|	dcat:keyword	|	radion:keyword	|	-	|	-	|
2.7 Frequency of Update	|	extra:update_frequency	|	-	|	-	|	-	|	dcat:accuralPeriodicity 	|	-	|	-	|	-	|
2.8 Title	|	dataset:title	|	-	|	-	|	sdo:name	|	dcterms:title	|	rdfs:label	|	-	|	-	|
2.9 Category	|	-	|	-	|	-	|	sdo:about	|	dcat:theme	|	dcterms:subject	|	-	|	-	|
3 Extent	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|
3.1 Spatial coverage	|	taxonomy:geographical_coverage	|	-	|	-	|	ds:spatialCoverage	|	dcterms:spatial	|	dcterms:spatial	|	-	|	-	|
3.2 Spatial Type	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|
3.3 Spatial Coordinates	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|
3.4 Geographic Region Name	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|
3.5 Geographic Bounding Box - Lower Left Corner  	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|
3.6 Bounding Box - Upper Right Corner  	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|
3.7 Bounding Box - Coordinate Reference System  	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|
3.8 Geographic Bounding Box - Dimensions  	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|
3.9 Temporal coverage	|	-	|	-	|	-	|	ds:temporalCoverage	|	dcterms:temporal	|	-	|	-	|	-	|
3.10 Temporal coverage starts	|	extra:temporal_coverage_from	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|
3.11 Temporal coverage ends	|	extra:temporal_coverage_to	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|
3.12 Temporal granularity	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|
3.13 Temporal granularity factor	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|
3.14 Periodicity of data(set) collection	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|
3.15 Periodicity of the production process	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|
3.16 Periodicity of the estimates	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|
3.17 Temporal and spatial comparability	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|
3.18 Periodicity of data dissemination	|	extra:update_frequency	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|
3.19 Data quality	|	-	|	-	|	-	|	-	|	dcat:dataQuality	|	-	|	-	|	-	|
3.20.X Reference period	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|
4. Supplemental Information	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|
4.1 Documentation URL - resource	|	resource:resource_type	|	-	|	-	|	-	|	dcat:dataDictionary 	|	-	|	-	|	-	|
5. Supplemental Information	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|
5.1 Licence	|	dataset:licence	|	-	|	-	|	-	|	dcterms:license	|	-	|	-	|	-	|
5.2 Copyright	|	-	|	-	|	-	|	sdo:copyrightHolder	|	-	|	-	|	-	|	-	|
5.3 Size	|	-	|	-	|	-	|	sdo:contentSize	|	dcat:size	|	-	|	-	|	-	|
5.4 URL - resource	|	rescource:url	|	-	|	-	|	sdo:contentUrl	|	dcat:accessURL	|	adms:accessURL	|	-	|	-	|
5.5 Homepage URL	|	-	|	-	|	-	|	sdo:url	|	foaf:homepage	|	-	|	-	|	-	|
5.6 Format - resource	|	resource:format	|	-	|	-	|	sdo:encodingFormat	|	dcterms:format	|	dcterms:format	|	-	|	-	|
5.7 Language	|	taxonomy:lanugage	|	-	|	-	|	sdo:inLanguage	|	dcterms:language	|	dcterms:language	|	-	|	-	|

