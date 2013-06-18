####Russian Federation Metadata

**Metadata Details**

Concept|Description|Front-end (human-readable)|National metadata schema|Back-end machine-readable|Required|Data Type|Format: pattern|Cardinality|Usage Notes
------- | -------- | ----- | ---- | ---------- | ---------|-------|-------|-------|------
1. *Contact information*  |  -  |    -  |	-	|	-	|	-	|	-	|	-	|	-	|	-	|
1.1 Person	|	Contact person’s name for the asset.	|	Ответственное лицо	|	-	|	-	|	Yes	|	xsd:string	|	"Last name" "First name" "Middle name" 	|	(1,1)	|	-
1.2 Contact Email - Publisher	|	Contact person’s email address.	|	Электронный адрес ответственного лица	|	-	|	-	|	Yes	|	xsd:string	|	Email address	|	(1,1)	|	-
1.2 Contact Email - Dataset	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-
1.3 Organisation (Owner)	|	The publishing agency.	|	Владелец набора данных	|	-	|	-	|	Yes	|	xsd:string	|	See Usage Notes	|	(1,1)	|	Departments and multi-unit agencies may use this field to describe which subordinate agency published this dataset.
1.4 Publisher	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-
1.5 Author	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-
1.6 Author Email	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-
1.7 Maintainer	|	-	|	Информация о субъекте, ответственном за обновление данных	|	-	|	-	|	No	|	xsd:string	|	"Last name" "First name" "Middle name" 	|	-	|	-
1.8 Maintainer Email	|	-	|	Электронная почта субъекта, ответственного за обновление данных	|	-	|	-	|	No	|	xsd:string	|	Email address	|	-	|	-
2. *Dataset Identification*	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-
2.1 Unique Identifier	|	A unique identifier for the dataset or API as maintained within an Agency catalog or database.	|	Идентификационный код 	|	-	|	-	|	Yes	|	xsd:string	|	"VAT identification number"-"short eng name"	|	(1,1)	|	This field allows third parties to maintain a consistent record for datasets even if title or URLs are updated. Agencies may integrate an existing system for maintaining unique identifiers or enter arbitrary characters for this field. However, each identifier must be unique across the agency’s catalog and remain fixed. 
2.2 Release Date	|	Date of formal issuance.	|	Дата первой публикации набора данных	|	-	|	-	|	Yes	|	Date	|	Date (DD.MM.YYYY)	|	(1,1)	|	-
2.2.R Release Date	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-
2.3 Modified	|	Most recent date on which the dataset was changed, updated or modified.	|	Дата последнего внесения изменений	|	-	|	-	|	Yes	|	Date	|	Date (DD.MM.YYYY)	|	(1,1)	|	-
2.3.R Modified	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-
2.4 Last Updated	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-
2.4.R Last Updated	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-
2.5 Description	|	Human-readable description (e.g., an abstract) with sufficient detail to enable a user to quickly understand whether the asset is of interest.	|	Описание набора данных	|	-	|	-	|	Yes	|	xsd:string	|	^[А-ЯЁа-яё0-9_-]{2,}$	|	(1,1)	|	-
2.6 Keyword	|	Tags (or keywords) help users discover your dataset, please include terms that would be used by technical and non-technical users.	|	Ключевые слова 	|	-	|	-	|	Yes	|	xsd:string	|	Separate keywords with commas.	|	(1,n)	|	Separate keywords with commas.
2.7 Frequency of Update	|	Frequency with which dataset is published.	|	Периодичность актуализации набора данных	|	-	|	-	|	Yes	|	See Usage Notes	|	See Usage Notes	|	(1,1)	|	Must be one of the following:  yearly,quarterly,monthly,daily, other
2.8 Title	|	Human-readable name of the asset. Should be in plain English and include sufficient detail to facilitate search and discovery.	|	Наименование набора данных	|	-	|	-	|	Yes	|	xsd:string	|	^[А-ЯЁа-яё0-9_-]{2,}$	|	(1,1)	|	-
2.9 Category	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-
3. *Extent*	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-
3.1 Spatial coverage	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-
3.2 Spatial Type	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-
3.3 Spatial Coordinates	|	-	|	Пространственные координаты	|	-	|	-	|	No	|	-	|	-	|	-	|	-
3.4 Geographic Region Name	|	-	|	Название региона	|	-	|	-	|	No	|	xsd:string	|	^[А-ЯЁа-яё0-9_-]{2,}$	|	-	|	-
3.5 Geographic Bounding Box - Lower Left Corner  	|	-	|	"Широта крайней южной точки Долгота крайней западной точки"	|	-	|	-	|	No	|	-	|	-	|	-	|	-
3.6 Bounding Box - Upper Right Corner  	|	-	|	"Широта крайней северной точки Долгота крайней восточной точки"	|	-	|	-	|	No	|	-	|	-	|	-	|	-
3.7 Bounding Box - Coordinate Reference System  	|	-	|	Система координат	|	-	|	-	|	No	|	-	|	-	|	-	|	-
3.8 Geographic Bounding Box - Dimensions  	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-
3.9 Temporal coverage	|	-	|	Длина временного ряда	|	-	|	-	|	No	|	-	|	-	|	-	|	-
3.10 Temporal coverage starts	|	-	|	Период действия: с	|	-	|	-	|	No	|	-	|	-	|	-	|	-
3.11 Temporal coverage ends	|	-	|	Период действия: по	|	-	|	-	|	No	|	-	|	-	|	-	|	-
3.12 Temporal granularity	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-
3.13 Temporal granularity factor	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-
3.14 Periodicity of data(set) collection	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-
3.15 Periodicity of the production process	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-
3.16 Periodicity of the estimates	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-
3.17 Temporal and spatial comparability	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-
3.18 Periodicity of data dissemination	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-
3.19 Data quality	|	-	|	Качество набора данных	|	-	|	-	|	No	|	-	|	-	|	-	|	-
3.20 Reference period	|	-	|	Отчетный период	|	-	|	-	|	No	|	-	|	-	|	-	|	-
4. *Supplemental Information*	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-
4.1 Documentation URL - resource	|	-	|	Гиперссылка (URL) на структуру набора данных	|	-	|	-	|	Yes	|	anyURI	|	-	|	(1,1)	|	-
5. *Distribution Information*	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-
5.1 Licence	|	-	|	Условия использования набора данных	|	-	|	-	|	No	|	xsd:string	|	^[А-ЯЁа-яё0-9_-]{2,}$	|	-	|	-
5.2 Copyright	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-
5.3 Size	|	-	|	Размер файла набора данных	|	-	|	-	|	 No	|	-	|	-	|	-	|	-
5.4 URL - resource	|	-	|	Ссылка (URL) на набор	|	-	|	-	|	Yes	|	anyURI	|	-	|	(1,1)	|	-
5.5 Homepage URL	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-
5.6 Format - resource	|	-	|	Формат	|	-	|	-	|	Yes	|	xsd:string	|	^[A-Z]{3,8}$	|	(1,1)	|	-
5.7 Language	|	-	|	Язык, используемый для документирования метаданных	|	-	|	-	|	No	|	-	|	-	|	-	|	-

Concept|'Other' (i.e. not one specific source|
------- | -------- |
Concept  |	Other (e.g. Dublin Core, Foaf, RDF, RDFa Lite, Microdata)	|
1. Contact information	|	-	|
1.1 Person	|	dcterms:publisher	|
1.2 Contact Email - Publisher	|	foaf:mbox	|
1.2 Contact Email - Dataset	|	-	|
1.3 Organisation (Owner)	|	dcterms:owner	|
1.4 Publisher	|	-	|
1.5 Author	|	-	|
1.6 Author Email	|	-	|
1.7 Maintainer	|	-	|
1.8 Maintainer Email	|	-	|
2. Dataset Identification	|	-	|
2.1 Unique Identifier	|	dcterms:identifier	|
2.2 Release Date	|	dcterms:created	|
2.2.R Release Date	|	-	|
2.3 Modified	|	dcterms:modified	|
2.3.R Modified	|	-	|
2.4 Last Updated	|	-	|
2.4.R Last Updated	|	-	|
2.5 Description	|	dcterms:description	|
2.6 Keyword	|	dcterms:subject	|
2.7 Frequency of Update	|	dcterms:valid	|
2.8 Title	|	dcterms:title	|
2.9 Category	|	-	|
3. *Extent*	|	-	|
3.1 Spatial coverage	|	-	|
3.2 Spatial Type	|	-	|
3.3 Spatial Coordinates	|	-	|
3.4 Geographic Region Name	|	-	|
3.5 Geographic Bounding Box - Lower Left Corner  	|	-	|
3.6 Bounding Box - Upper Right Corner  	|	-	|
3.7 Bounding Box - Coordinate Reference System  	|	-	|
3.8 Geographic Bounding Box - Dimensions  	|	-	|
3.9 Temporal coverage	|	-	|
3.10 Temporal coverage starts	|	-	|
3.11 Temporal coverage ends	|	-	|
3.12 Temporal granularity	|	-	|
3.13 Temporal granularity factor	|	-	|
3.14 Periodicity of data(set) collection	|	-	|
3.15 Periodicity of the production process	|	-	|
3.16 Periodicity of the estimates	|	-	|
3.17 Temporal and spatial comparability	|	-	|
3.18 Periodicity of data dissemination	|	-	|
3.19 Data quality	|	-	|
3.20.Reference period	|	-	|
4. *Supplemental Information*	|	-	|
4.1 Documentation URL - resource	|	dcterms:source	|
5. *Distribution Information*	|	-	|
5.1 Licence	|	-	|
5.2 Copyright	|	-	|
5.3 Size	|	-	|
5.4 URL - resource	|	dcterms:source	|
5.5 Homepage URL	|	-	|
5.6 Format - resource	|	dcterms:format	|
5.7 Language	|	-	|


