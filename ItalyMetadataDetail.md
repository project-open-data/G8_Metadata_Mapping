####Italy Metadata

**Where to Find Data**

Where to find: The website [dati.gov.it](http://www.data.gov.it) collects and publishes datasets published in Public Administrations' open data repositories. The website publishes news and infographics about open data diffusion in Italy. There is also a section Applicazioni which is a repository of applications released by using open data published by Public Administrations.

Licensing: All material of data.gov.it is subject to the CC BY 3.0 IT license

Contact: TBC

Next planned change: Integration with CKAN2 for data harvesting (30 September 2013)

**Metadata Details**

Concept|Description|Front-end (human-readable)|National metadata schema|Back-end machine-readable|Required|Data Type|Format: pattern|Cardinality|Usage Notes
------- | -------- | ----- | ---- | ---------- | ---------|-------|-------|-------|------
1. *Contact information*  |	-	|	-	|	-	|	-	|	Yes	|	String	|	^[a-z0-9_-]{2,}$	|	(1,1)	|
1.1 Person	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|
1.2 Contact Email - Publisher	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|
1.2 Contact Email - Dataset	|	-	|	Mail del Funzionario/Unità organizzativa	|	-	|	field_email_rif	|	no	|	-	|	-	|	-	|
1.3 Organisation (Owner)	|	-	|	Ente gestore	|	-	|	field_ente_gestore	|	no	|	-	|	-	|	-	|
1.4 Publisher	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|
1.5 Author	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|
1.6 Author Email	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|
1.7 Maintainer	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|
1.8 Maintainer Email	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|
2. *Dataset Identification*	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|
2.1 Unique Identifier	|	-	|	ID univoco dataset	|	-	|	nid	|	yes	|	-	|	-	|	-	|
2.2 Release Date	|	-	|	Data caricamento	|	-	|	field_data_load	|	no	|	-	|	-	|	-	|
2.2.R Release Date	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|
2.3 Modified	|	-	|	Data di aggiornamento	|	-	|	field_data_last_update	|	no	|	-	|	-	|	-	|
2.3.R Modified	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|
2.4 Last Updated	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|
2.4.R Last Updated	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|
2.5 Description	|	-	|	Descrizione	|	-	|	body	|	yes	|	-	|	-	|	-	|
2.6 Keyword	|	-	|	tag liberi	|	-	|	field_tag	|	no	|	-	|	-	|	-	|
2.7 Frequency of Update	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|
2.8 Title	|	-	|	Titolo	|	-	|	title	|	yes	|	-	|	-	|	-	|
2.9 Category	|	-	|	Area tematica	|	-	|	field_areatematica	|	no	|	-	|	-	|	-	|
2. *Extent*  |	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|
3. 3.1 Spatial coverage	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|
3.2 Spatial Type	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|
3.3 Spatial Coordinates	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|
3.4 Geographic Region Name	|	-	|	Regione	|	-	|	field_regione	|	no	|	-	|	-	|	-	|
3.5 Geographic Bounding Box - Lower Left Corner  	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|
3.6 Bounding Box - Upper Right Corner  	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|
3.7 Bounding Box - Coordinate Reference System  	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|
3.8 Geographic Bounding Box - Dimensions  	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|
3.9 Temporal coverage	|	-	|	Periodo validità	|	-	|	field_data_from_to	|	no	|	-	|	-	|	-	|
3.10 Temporal coverage starts	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|
3.11 Temporal coverage ends	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|
3.12 Temporal granularity	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|
3.13 Temporal granularity factor	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|
3.14 Periodicity of data(set) collection	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|
3.15 Periodicity of the production process	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|
3.16 Periodicity of the estimates	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|
3.17 Temporal and spatial comparability	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|
3.18 Periodicity of data dissemination	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|
3.19 Data quality	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|
3.20.X Reference period	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|
4.*Supplemental Information*	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|
4.1 Documentation URL - resource	|	-	|	Note	|	-	|	field_note	|	no	|	-	|	-	|	-	|
5. *Distribution Information*	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|
5.1 Licence	|	-	|	Licenza	|	-	|	field_licenza	|	no	|	-	|	-	|	-	|
5.2 Copyright	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|
5.3 Size	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|
5.4 URL - resource	|	-	|	URL pagina dataset	|	-	|	field_url_dataset	|	yes	|	-	|	-	|	-	|
5.5 Homepage URL	|	-	|	Home page ente	|	-	|	field_site_url_ente	|	no	|	-	|	-	|	-	|
5.6 Format - resource	|	-	|	Formato dati	|	-	|	field_formato	|	no	|	-	|	-	|	-	|
5.7 Language	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|


**Mapping**
Please find the metadata mapping index between G8 nations [here](https://github.com/nsinai/G8_Metadata_Mapping/blob/master/index.md).

**Feedback**
Please give feedback on this mapping - you can fill out a [short survey (5 questions)](http://www.surveymonkey.com/s/CCM3F2C) or a [longer survey (10 questions)](http://www.surveymonkey.com/s/N2ZMP7K).


