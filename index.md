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
1. Contact information |	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|
1.1.H Person	|	Contact Name	|	-	|	-	|	-	|	Contact Name	|	Ansprechpartner	|	-	|	-	|	Ответственное лицо	|
1.1.M Person	|	maintainer	|	-	|	-	|	-	|	contact_name	|	extras->contacts->name	|	-	|	-	|	Responsible	|
1.2.H Contact Email - Publisher	|	Contact Email	|	Email / phone	|	Page producteur	|	Email	|	Contact / Email	|	Ansprechpartner: E-Mail	|	-	|	-	|	Электронный адрес ответственного лица	|
1.2.M Contact Email - Publishers	|	maintainer_email	|	Package.contact-email / contact-phone	|	-	|	author_email	|	contact_email	|	extras->contacts->email	|	-	|	-	|	Responsible Email	|
1.2.H Contact Email - Dataset	|	-	|	Email / phone	|	Poser la première question/Poser une question	|	-	|	-	|	-	|	-	|	Mail del Funzionario/Unità organizzativa	|	-	|
1.2.M Contact Email - Dataset	|	-	|	Group.contact-email / contact-phone	|	-	|	-	|	-	|	-	|	-	|	field_email_rif	|	-	|
1.3.H Organisation (Owner)	|	Publisher	|	Enquiries / FOI Contact	|	Producteur de données	|	(=Publisher)	|	Contact Point	|	(= Maintainer OR author)	|	-	|	Ente gestore	|	Владелец набора данных	|
1.3.M Organisation (Owner)	|	owner_org	|	Package.contact-name / Package.foi-name / Group.contact-name / Group.foi-name	|	Producteur de données	|	owner_org	|	-	|	-	|	-	|	field_ente_gestore	|	Data owner	|
1.4.H Publisher	|	-	|	Publisher	|	Producteur de données	|	Publisher	|	Publisher	|	(= Author)	|	-	|	-	|	-	|
1.4.M Publisher	|	-	|	Group	|	Producteur de données	|	owner_org	|	published_by	|	-	|	-	|	-	|	-	|
1.5.H Author	|	-	|	-	|	Producteur de données	|	(=Publisher)	|	Contact Name	|	Veröffentlichende Stelle	|	作成者 	|	-	|	-	|
1.5.M Author	|	-	|	-	|	Producteur de données	|	owner_org	|	-	|	author	|	author	|	-	|	-	|
1.6.H Author Email	|	-	|	-	|	-	|	(=Email)	|	-	|	Veröffentlichende Stelle: E-Mail	|	作成者のメールアドレス	|	-	|	-	|
1.6.M Author Email	|	-	|	-	|	-	|	author_email	|	-	|	author_email	|	author_email	|	-	|	-	|
1.7.H Maintainer	|	-	|	-	|	Producteur de données	|	(=Email)	|	Contact Name	|	Datenverantwortliche Stelle	|	メンテナー	|	-	|	Информация о субъекте, ответственном за обновление данных	|
1.7.M Maintainer	|	-	|	-	|	Producteur de données	|	electronicMailAddress	|	-	|	maintainer	|	maintainer	|	-	|	Maintainer	|
1.8.H Maintainer Email	|	-	|	-	|	-	|	(=Email)	|	-	|	Datenverantwortliche Stelle: E-Mail	|	メンテナーのメールアドレス	|	-	|	Электронная почта субъекта, ответственного за обновление данных	|
1.8.M Maintainer Email	|	-	|	-	|	-	|	author_email	|	-	|	maintainer_email	|	maintainer_email	|	-	|	Maintainer Email	|
2. Dataset Identification	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|
2.1.H Unique Identifier	|	Unique Identifier	|	URI	|	URL	|	File Identifier	|	Identifier	|	Name	|	URLの一部	|	ID univoco dataset	|	Идентификационный код 	|
2.1.M Unique Identifier	|	id	|	name	|	PSI	|	id	|	identifier	|	name	|	name	|	nid	|	-	|
2.2.H Release Date	|	Release Date	|	Added to data.gov.uk	|	Publié le 	|	Date Published	|	Created	|	Veröffentlichungsdatum	|	-	|	Data caricamento	|	Дата первой публикации набора данных	|
2.2.M Release Date	|	-	|	metadata_created	|	Date de publication	|	date_published	|	release_date	|	" (extras->dates->role = ""veroeffentlicht""):
extras->dates->date"	|	-	|	field_data_load	|	Date of first publication	|
2.2.H.R Release Date	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|
2.2.M.R Release Date	|	-	|	-	|	-	|	-	|	created	|	-	|	-	|	-	|	-	|
2.3.H Modified	|	-	|	Modified on data.gov.uk	|	Modifé le	|	Date Modified	|	Modified date	|	Stand Metadaten 	|	-	|	Data di aggiornamento	|	Дата последнего внесения изменений	|
2.3.M Modified	|	-	|	metadata_modified	|	Date de changement de statut	|	modified	|	modified_date	|	"(extras->dates->role = ""aktualisiert"")
extras->dates->date"	|	-	|	field_data_last_update	|	-	|
2.3.H.R Modified	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|
2.3.M.R Modified	|	-	|	-	|	-	|	-	|	last_modified	|	-	|	-	|	-	|	-	|
2.4.H Last Updated	|	Last Update	|	-	|	-	|	(=Date Modified)	|	Last modified	|	[= Modified (date that this dataset was changed)]	|	-	|	-	|	-	|
2.4.M Last Updated	|	revision_timestamp	|	-	|	-	|	modified	|	-	|	-	|	-	|	-	|	-	|
2.4.H.R Last Updated	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|
2.4.M.R Last Updated	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|
2.5.H Description	|	Description	|	Description	|	Description	|	Description	|	Description	|	Beschreibung	|	説明	|	Descrizione	|	Описание набора данных	|
2.5.M Description	|	notes	|	notes	|	Description	|	notes	|	description	|	notes	|	notes	|	body	|	Data description	|
2.6.H Keyword	|	Tags	|	Tags	|	Mots clés	|	Keywords  	|	Keywords	|	Schlagwörter	|	-	|	tag liberi	|	Ключевые слова 	|
2.6.M Keyword	|	tags	|	PackageTag	|	Mots clés / thématiques	|	keywords	|	keyword_string	|	tags	|	-	|	field_tag	|	Keywords	|
2.7.H Frequency of Update	|	-	|	Frequency of update	|	Fréquence de mise à jour	|	Frequency	|	-	|	-	|	-	|	-	|	Периодичность актуализации набора данных	|
2.7.M Frequency of Update	|	-	|	 frequency-of-update (UKLP only)	|	Fréquence de mise à jour	|	maintenance_and_update_frequency	|	type_of_dataset	|	-	|	-	|	-	|	-	|
2.8.H Title	|	Title	|	Title	|	Titre	|	Title	|	Title	|	Titel	|	タイトル	|	Titolo	|	Наименование набора данных	|
2.8.M Title	|	title	|	title	|	Nom	|	title	|	title	|	title	|	title	|	title	|	Data title	|
2.9.H Category	|	Category	|	National Statistics	|	Mots clés	|	"Subject 
Topic Category"	|		|		|		|	Area tematica	|		|
2.9.M Category	|	groups	|		|		|	"subject
topic_category"	|		|		|		|	field_areatematica	|		|
3. Extent	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|
3.1.H Spatial coverage	|	Spatial	|	Dataset Extent	|	Couverture géographique	|	Spatial	|	Geographical coverage	|	Geographische Abdeckung	|	-	|	-	|	-	|
3.1.M Spatial coverage	|	spatial	|	-	|	Couverture géographique	|	spatial	|	geographical_coverage	|	(see below)	|	-	|	-	|	-	|
3.2.H Spatial Type	|	-	|	-	|	-	|	Spatial Representation Type	|	-	|	Art der Form	|	-	|	-	|	-	|
3.2.M Spatial Type	|	-	|	-	|	-	|	spatial_representation_type	|	-	|	extras->spatial->type	|	-	|	-	|	-	|
3.3.H Spatial Coordinates	|	-	|	Dataset Extent	|	-	|	(=Spatial)	|	-	|	Koordinaten-Liste	|	-	|	-	|	Пространственные координаты	|
3.3.M Spatial Coordinates	|	-	|	spatial	|	-	|	spatial	|	-	|	extras->spatial->coordinates	|	-	|	-	|	Spatial coordinates	|
3.4.H Geographic Region Name	|	-	|	-	|	-	|	Geographic Region	|	-	|	Abgedecktes Gebiet	|	-	|	Regione	|	Название региона	|
3.4.M Geographic Region Name	|	-	|	-	|	-	|	geographic_region	|	-	|	extras->spatial_text	|	-	|	field_regione	|	Geographic Region Name	|
3.5.H Geographic Bounding Box - Lower Left Corner  	|	-	|	Latitude / Longitude	|	-	|	(=Spatial)	|	-	|	-	|	-	|	-	|	"Широта крайней южной точки
Долгота крайней западной точки"	|
3.5.M Geographic Bounding Box - Lower Left Corner  	|	-	|	bbox-west-long, bbox-south-lat	|	-	|	spatial	|	-	|	-	|	-	|	-	|	-	|
3.6.H Bounding Box - Upper Right Corner  	|	-	|	Latitude / Longitude	|	-	|	(=Spatial)	|	-	|	-	|	-	|	-	|	"Широта крайней северной точки
Долгота крайней восточной точки"	|
3.6.M Bounding Box - Upper Right Corner  	|	-	|	bbox-east-long, bbox-north-lat	|	-	|	spatial	|	-	|	-	|	-	|	-	|	-	|
3.7.H Bounding Box - Coordinate Reference System  	|	-	|	Spatial reference system	|	-	|	(=Spatial)	|	-	|	-	|	-	|	-	|	Система координат	|
3.7.M Bounding Box - Coordinate Reference System  	|	-	|	spatial-reference-system	|	-	|	spatial	|	-	|	-	|	-	|	-	|	-	|
3.8.H Geographic Bounding Box - Dimensions  	|	-	|	-	|	-	|	(=Spatial)	|	-	|	-	|	-	|	-	|	-	|
3.8.M Geographic Bounding Box - Dimensions  	|	-	|	-	|	-	|	spatial	|	-	|	-	|	-	|	-	|	-	|
3.9.H Temporal coverage	|	temporal	|	Temporal coverage	|	Période	|	(=Temporal)	|	Temporal coverage	|	Zeitliche Abdeckung	|	-	|	Periodo validità	|	Длина временного ряда	|
3.9.M Temporal coverage	|	-	|	-	|	(Fin de la période couverte par les données)+(Début de la période couverte par les données)	|	time_period_coverage_start/time_period_coverage_end	|	-	|	(see below)	|	-	|	field_data_from_to	|	The length of time series	|
3.10.H Temporal coverage starts	|	-	|	-	|	(Période)	|	Time Period Coverage Start  	|	Temporal coverage from	|	Zeitliche Abdeckung: Start-Datum	|	-	|	-	|	Период действия: с	|
3.10.M Temporal coverage starts	|	-	|	 temporal_coverage-from	|	Début de la période couverte	|	time_period_coverage_start	|	temporal_coverage_from	|	extras->temporal_coverage_from	|	-	|	-	|	Validity period: from	|
3.11.H Temporal coverage ends	|	-	|	-	|	(Période)	|	Time Period Coverage End	|	Temporal coverage to	|	Zeitliche Abdeckung: End-Datum	|	-	|	-	|	Период действия: по	|
3.11.M Temporal coverage ends	|	-	|	 temporal_coverage-to	|	Fin de la période couverte	|	time_period_coverage_end	|	temporal_coverage_to	|	extras->temporal_coverage_to	|	-	|	-	|	Validity period: to	|
3.12.H Temporal granularity	|	Granularity	|	-	|	-	|	-	|	temporal coverage / granularity	|	Zeitliche Auflösung	|	-	|	-	|	-	|
3.12.M Temporal granularity	|	-	|	-	|	-	|	-	|	-	|	extras->temporal_granularity	|	-	|	-	|	-	|
3.13.H Temporal granularity factor	|	-	|	-	|	-	|	-	|	-	|	Faktor für die zeitliche Auflösung	|	-	|	-	|	-	|
3.13.M Temporal granularity factor	|	-	|	-	|	-	|	-	|	-	|	extras->temporal_granularity_factor	|	-	|	-	|	-	|
3.14.H Periodicity of data(set) collection	|	-	|	-	|	-	|	(=Frequency)	|	-	|	-	|	-	|	-	|	-	|
3.14.M Periodicity of data(set) collection	|	-	|	-	|	-	|	maintenance_and_update_frequency	|	accural_periodicity	|	-	|	-	|	-	|	-	|
3.15.H Periodicity of the production process	|	-	|	-	|	-	|	(=Frequency)	|	-	|	-	|	-	|	-	|	-	|
3.15.M Periodicity of the production process	|	-	|	-	|	-	|	maintenance_and_update_frequency	|	-	|	-	|	-	|	-	|	-	|
3.16.H Periodicity of the estimates	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|
3.16.M Periodicity of the estimates	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|
3.17.H Temporal and spatial comparability	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|
3.17.M Temporal and spatial comparability	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|
3.18.H Periodicity of data dissemination	|	Frequency	|	-	|	-	|	-	|	acrrual periodicity	|	-	|	-	|	-	|	-	|
3.18.M Periodicity of data dissemination	|	-	|	-	|	-	|	-	|	accural_periodicity	|	-	|	-	|	-	|	-	|
3.19.H Data quality	|	Data Quality	|	Openness score	|	-	|	-	|	-	|	-	|	-	|	-	|	Качество набора данных	|
3.19.M Data quality	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	dataQuality	|
3.X.H Reference period	|	-	|	-	|	-	|	(=Temporal)	|	-	|	-	|	-	|	-	|	Отчетный период	|
3.X.M Reference period	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	Reference period	|
4. Supplemental Information	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|
4.1.H Documentation URL - resource	|	Related Documents	|	Additional Resources	|	Annexe	|	(=Resource Type)	|	Documentation / URL	|	Website	|	-	|	Note	|	Гиперссылка (URL) на структуру набора данных	|
4.1.M Documentation URL - resource	|	resources	|	Resource.descriptoin, Resource.url, Resource.format	|	Ressource Annexe	|	resource_type	|	url	|	url	|	-	|	field_note	|	-	|
5. Distribution Information	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|
5.1.H Licence	|	License	|	Licence	|	Licence	|	Licence	|	Licence	|	Nutzungsbestimmungen	|	ライセンス	|	Licenza	|	Условия использования набора данных	|
5.1.M Licence	|	license_id	|	license_id	|	Licence	|	licence_id	|	license_id	|	license_id	|	license_id	|	field_licenza	|	License	|
5.2.H Copyright	|	-	|	-	|	-	|	(=Licence)	|	-	|	-	|	-	|	-	|	-	|
5.2.M Copyright	|	-	|	-	|	-	|	licence_id	|	-	|	-	|	-	|	-	|	-	|
5.3.H Size	|	Size	|	-	|	Taille	|	Size	|	Size	|	-	|	-	|	-	|	Размер файла набора данных	|
5.3.M Size	|	-	|	-	|	taille	|	size	|	-	|	-	|	-	|	-	|	Size	|
5.4.M URL - resource	|	-	|	URL	|	Cible du bouton de téléchargement	|	URL	|	URL	|	Link	|	ホームページ	|	URL pagina dataset	|	Ссылка (URL) на набор	|
5.4.H URL - resource	|	-	|	Resource.url	|	"chargement de fichier"+"URL d'accès"	|	url	|	url	|	resources->url	|	url	|	field_url_dataset	|	Data URL	|
5.5.H Homepage URL	|	Homepage URL	|	Home	|	Accueil 	|	Homepage URL	|	URL/HOME	|		|	ホームページ【再掲】	|	Home page ente	|		|
5.5.M Homepage URL	|	url	|		|		|	url	|		|		|	url	|	field_site_url_ente	|		|
5.6.H Format - resource	|	Format	|	Format	|	Format	|	Format	|	Format	|	Format	|	-	|	Formato dati	|	Формат	|
5.6.M Format - resource	|	res_format	|	Resource.format	|	format	|	format	|	format	|	resources->format	|	-	|	field_formato	|	Format 	|
5.7.H Language	|	Language	|	-	|	Langue	|	Language	|	language	|	Sprache	|	-	|	-	|	Язык, используемый для документирования метаданных	|
5.7.M Language	|	-	|	-	|	Langue du jeu de données	|	language	|	language	|	resources->language	|	-	|	-	|	Language	|


**Feedback**
Please give feedback on this mapping - you can fill out a [short survey (5 questions)](http://www.surveymonkey.com/s/CCM3F2C) or a longer one (10 questions).
