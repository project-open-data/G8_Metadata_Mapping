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

