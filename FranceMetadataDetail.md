####France Metadata

**Where to Find Data**

Where to find: [Data.gouv.fr](http://www.data.gouv.fr) is the national Open Data platform for the French government. It acts as a unique access point to all national-level open government data.

Licensing: [Licence Ouverte/Open Licence](http://www.data.gouv.fr/Licence-Ouverte-Open-Licence)

Contact: Romain LACOMBE (romain.lacombe@pm.gouv.fr)

Metadata last updated: 5th December 2011

Next planned change: None planned

**Metadata Details**

Concept|Description|Front-end (human-readable)|National metadata schema|Back-end machine-readable|Required|Data Type|Format: pattern|Cardinality|Usage Notes
------- | -------- | ----- | ---- | ---------- | ---------|-------|-------|-------|------
1. *Contact information*  |	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|
1.1 Person	|	-	|	-	|	Not used	|	-	|	-	|	-	|	-	|	-	|	-	|
1.2 Contact Email - Publisher	|	Page producteur	|	-	|	Not used - however,  each Publisher organisation has a page on data.gouv.fr with links to their web presence through which users can contact them.	|	-	|	yes	|	-	|	one choice among many 	|	(1,1)	|	Must correspond to one organisation among a list of data producers maintained by the Etalab (data.gouv.fr) team.	|
1.2 Contact Email - Dataset	|	Poser la première question/Poser une question	|	-	|	Not used - however, users can register and create an account on data.gouv.fr through which they can ask questions on each dataset, which are made public and are notified to the civil servant tasked with publishing and maintaining the dataset inside the Publisher organisation.	|	-	|	no	|	-	|	-	|	(0,n)	|	Questions and answers from users with a registered account on data.gouv.fr pertaining to this specific dataset.	|
1.3 Organisation (Owner)	|	Producteur de données	|	Producteur de données	|	All of the concepts above are represented by only one metadata field on data.gouv.fr: 'Organisation'. This field refers to the organisation, ministerial department, office, agency, local authority, or any other type of public sector body which produces, maintains and releases the dataset. This field maps to a list of data producers maintained by the Etalab (data.gouv.fr) team.	|	-	|	yes	|	See Usage notes	|	one choice among many	|	(1,1)	|	Must correspond to one organisation among a list of data producers maintained by the Etalab (data.gouv.fr) team.	|
1.4 Publisher	|	Producteur de données	|	Producteur de données	|	See Organisation	|	-	|	yes	|	See below	|	one choice among many	|	(1,1)	|	See below	|
1.5 Author	|	Producteur de données	|	Producteur de données	|	See Organisation	|	-	|	yes	|	See below	|	one choice among many	|	(1,1)	|	See below	|
1.6 Author Email	|	-	|	-	|	Not used	|	-	|	-	|	-	|	-	|	-	|	-	|
1.7 Maintainer	|	Producteur de données	|	Producteur de données	|	See Organisation	|	-	|	yes	|	See below	|	one choice among many	|	(1,1)	|	See below	|
1.8 Maintainer Email	|	-	|	-	|	Not used	|	-	|	-	|	-	|	-	|	-	|	-	|
2. *Dataset Identification*	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|
2.1 Unique Identifier	|	(Not used - apparent in URL scheme)	|	PSI	|	Machine-readable string that uniquely identifies the dataset online.	|	-	|	yes	|	See Usage Notes	|	URI string	|	(1,1)	|	A Unique Resource Identifier (URI) string is automatically generated when a dataset is registered. It uniquely maps to a dataset, is used for the URL scheme of data.gouv.fr and cannot be modified.	|
2.2 Release Date	|	Publié le 	|	Date de publication	|	Date at which this dataset was first released.	|	-	|	yes	|	Date	|	dd/mm/yyyy	|	(1,1)	|	Date at which the dataset was first released on data.gouv.fr.	|
2.2.R Release Date	|	-	|	-	|	Not used - see above	|	-	|	-	|	-	|	-	|	-	|	-	|
2.3 Modified	|	Modifé le	|	Date de changement de statut	|	Date at which this dataset was last updated.	|	-	|	yes	|	Date	|	dd/mm/yyyy	|	(1,1)	|	Date at which the dataset was last updated on data.gouv.fr.	|
2.3.R Modified	|	-	|	-	|	Not used - see above	|	-	|	-	|	-	|	-	|	-	|	-	|
2.4 Last Updated	|	-	|	-	|	Not used - see above	|	-	|	-	|	-	|	-	|	-	|	-	|
2.4.R Last Updated	|	-	|	-	|	Not used - see above	|	-	|	-	|	-	|	-	|	-	|	-	|
2.5 Description	|	Description	|	Description	|	The civil servants tasked with publishing and maintaining the dataset inside the Publisher organisation write a textual description of the dataset before it is released. It explains what the dataset is about, how it can be read and what the different columns, fields or values mean.	|	-	|	yes	|	string	|	free text	|	(1,1)	|	Free text.	|
2.6 Keyword	|	Mots clés	|	Mots clés / thématiques	|	Data publishers describe the dataset with a cloud of tags which may be either free-text keywords or keywords from the European standard vocabulary on public sector concepts (EUROVOC).	|	-	|	yes	|	See Usage Notes	|	tag cloud	|	(0,n)	|	Either free text or keywords from a controled vocabulary (EUROVOC).	|
2.7 Frequency of Update	|	Fréquence de mise à jour	|	Fréquence de mise à jour	|	This describes how often data users can expect the dataset to be updated.	|	-	|	yes	|	See Usage Notes	|	one choice among many	|	(1,1)	|	Must be one of the following: annuelle (annual), au fil de l'eau (go-with-the-flow), bimensuelle (twice per month), bimestrielle (every two months), hebdomadaire (weekly), journalier (daily), mensuelle (monthly), semestrielle (every six months), temps réel (real-time), trimestrielle (every three months)	|
2.8 Title	|	Titre	|	Nom	|	Short title of the dataset.	|	-	|	yes	|	string	|	free text	|	(1,1)	|	Title aimed at making the content of the dataset quickly understandable by users.	|
2.9 Category	|	Mots clés	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|
3 *Extent*	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|
3.1 Spatial coverage	|	Couverture géographique	|	Couverture géographique	|	The spatial coverage of the dataset is described as a reference to one of the administrative sub-divisions of the French territory, listed through the National Statistics Institute (INSEE)'s Official Geographic Code (COG - Code Officiel Géographique). 	|	-	|	yes	|	See Usage Notes	|	territorial administrative subdivision	|	(1,1)	|	Controled vocabulary: maps to one administrative territorial subdivision of INSEE's COG referential. These can be a "commune" (one of the 36,000+ French localities), a "département" (one of the 101 departments) or "région" (one of the 27 regions), or any intermediate subdivision.	|
3.2 Spatial Type	|	-	|	-	|	Not used	|	-	|	-	|	-	|	-	|	-	|	-	|
3.3 Spatial Coordinates	|	-	|	-	|	Not used	|	-	|	-	|	-	|	-	|	-	|	-	|
3.4 Geographic Region Name	|	-	|	-	|	Not used	|	-	|	-	|	-	|	-	|	-	|	-	|
3.5 Geographic Bounding Box - Lower Left Corner  	|	-	|	-	|	Not used	|	-	|	-	|	-	|	-	|	-	|	-	|
3.6 Bounding Box - Upper Right Corner  	|	-	|	-	|	Not used	|	-	|	-	|	-	|	-	|	-	|	-	|
3.7 Bounding Box - Coordinate Reference System  	|	-	|	-	|	Not used	|	-	|	-	|	-	|	-	|	-	|	-	|
3.8 Geographic Bounding Box - Dimensions  	|	-	|	-	|	Not used	|	-	|	-	|	-	|	-	|	-	|	-	|
3.9 Temporal coverage	|	Période	|	(Fin de la période couverte par les données)+(Début de la période couverte par les données)	|	Period which the dataset covers.	|	-	|	yes	|	See Usage Notes	|	dd/mm/yyyy - dd/mm/yyyy	|	(2,2)	|	A period is defined by a start date and an end date.	|
3.10 Temporal coverage starts	|	(Période)	|	"Début de la période couverte"	|	See Temporal coverage	|	-	|	yes	|	Date	|	dd/mm/yyyy	|	(1,1)	|	Start of the temporal coverage.	|
3.11 Temporal coverage ends	|	(Période)	|	"Fin de la période couverte"	|	See Temporal coverage	|	-	|	yes	|	Date	|	dd/mm/yyyy	|	(1,1)	|	End of the temporal coverage.	|
3.12 Temporal granularity	|	-	|	-	|	Not used	|	-	|	-	|	-	|	-	|	-	|	-	|
3.13 Temporal granularity factor	|	-	|	-	|	Not used	|	-	|	-	|	-	|	-	|	-	|	-	|
3.14 Periodicity of data(set) collection	|	-	|	-	|	See Frequency of update	|	-	|	-	|	-	|	-	|	-	|	-	|
3.15 Periodicity of the production process	|	-	|	-	|	See Frequency of update	|	-	|	-	|	-	|	-	|	-	|	-	|
3.16 Periodicity of the estimates	|	-	|	-	|	See Frequency of update	|	-	|	-	|	-	|	-	|	-	|	-	|
3.17 Temporal and spatial comparability	|	-	|	-	|	Not used	|	-	|	-	|	-	|	-	|	-	|	-	|
3.18 Periodicity of data dissemination	|	-	|	-	|	See Frequency of update	|	-	|	-	|	-	|	-	|	-	|	-	|
3.19 Data quality	|	-	|	-	|	Not used	|	-	|	-	|	-	|	-	|	-	|	-	|
3.20 Reference period	|	-	|	-	|	See Temporal coverage	|	-	|	-	|	-	|	-	|	-	|	-	|
4. *Supplemental Information*	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|
4.1 Documentation URL - resource	|	Annexe	|	Ressource Annexe	|	URL of any resources, technical annexes or descriptive documents produced by the Publisher organisation which may make it easier to understand and reuse the dataset.	|	-	|	no	|	-	|	URL list	|	(0,n)	|	List of URLs listed by the data publisher.	|
5. *Distribution Information*	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|
5.1 Licence	|	Licence	|	Licence	|	Licence granting rights and listing the responsibilities of both the data user and the data publisher. By default, public datasets are released on data.gouv.fr under the French Government's "Licence Ouverte/Open Licence" [URL: http://www.data.gouv.fr/Licence-Ouverte-Open-Licence].	|	-	|	yes	|	-	|	one choice among many	|	(1,1)	|	By default, maps to Etalab's "Licence Ouverte/Open Licence".	|
5.2 Copyright	|	-	|	-	|	Not used.	|	-	|	-	|	-	|	-	|	-	|	-	|
5.3 Size	|	Taille	|	taille	|	File size.	|	-	|	yes	|	-	|	int	|	(1,1)	|	File size in kB, MB or GB.	|
5.4 URL - resource	|	Cible du bouton de téléchargement	|	"chargement de fichier" and "URL d'accès"	|	Direct link to the dataset file allowing users to download the file.	|	-	|	yes	|	-	|	URL	|	(1,1)	|	Deep link for direct download.	|
5.5 Homepage URL	|	Accueil 	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|
5.6 Format - resource	|	Format	|	format	|	Type of format (e.g. CSV, RDF, etc.)	|	-	|	yes	|	See Usage Notes	|	one choice among many	|	(1,1)	|	Must be one of the following: CSV, DOC, DOCX, HTML, JSON, KML, ODS, ODT, PDF, RDF, RTF, SHP, TXT, XLS, XLSX, XML, XSD	|
5.7 Language	|	Langue	|	Langue du jeu de données	|	Language in which the dataset is produced and collected (French by default).	|	-	|	yes	|	-	|	one choice among many	|	(1,1)	|	By default: French.	|



**Mappings to Other Vocabs**

Concept|CKAN - Level 1|CKAN - Level 2|CKAN - Level 3|Schema.org|DCAT|ADMS|VoID|Other (e.g. Dublin Core, Foaf, RDF, RDFa Lite)|
------- | -------- | ----- | ---- | ---------- | ---------|-------|-------|-------|------
1. *Contact information*  |	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|
1.1 Person	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|
1.2 Contact Email - Publisher	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|
1.2 Contact Email - Dataset	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|
1.3 Organisation (Owner)	|	-	|	-	|	-	|	sdo:Organization	|	foaf:Organization	|	-	|	-	|	dcterms:creator	|
1.4 Publisher	|	-	|	-	|	-	|	sdo:publisher	|	dcterms:publisher	|	dcterms:publisher	|	-	|	-	|
1.5 Author	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|
1.6 Author Email	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|
1.7 Maintainer	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|
1.8 Maintainer Email	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|
2. *Dataset Identification*	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|
2.1 Unique Identifier	|	-	|	-	|	-	|	-	|	dcterms:identifier	|	-	|	-	|	-	|
2.2 Release Date	|	-	|	-	|	-	|	sdo:datePublished	|	dcterms:issued	|	dcterms:created	|	-	|	dcterms:issued	|
2.2.R Release Date	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|
2.3 Modified	|	-	|	-	|	-	|	sdo:dateModified	|	dcterms:modified	|	dcterms:modified	|	-	|	http://data.gouv.fr/onto#statutChanged	|
2.3.R Modified	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|
2.4 Last Updated	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|
2.4.R Last Updated	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|
2.5 Description	|	-	|	-	|	-	|	sdo:description	|	dcterms:description	|	dcterms:description	|	-	|	dcterms:description	|
2.6 Keyword	|	-	|	-	|	-	|	sdo:keywords	|	dcat:keyword	|	radion:keyword	|	-	|	dc:subject et http://data.gouv.fr/onto#eurovocSubject	|
2.7 Frequency of Update	|	-	|	-	|	-	|	-	|	dcat:accuralPeriodicity 	|	-	|	-	|	dcterms:accrualPeriodicity	|
2.8 Title	|	-	|	-	|	-	|	sdo:name	|	dcterms:title	|	rdfs:label	|	-	|	rdfs:label	|
2.9 Category	|	-	|	-	|	-	|	sdo:about	|	dcat:theme	|	dcterms:subject	|	-	|	-	|
3 *Extent*	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|
3.1 Spatial coverage	|	-	|	-	|	-	|	ds:spatialCoverage	|	dcterms:spatial	|	dcterms:spatial	|	-	|	dcterms:spatial	|
3.2 Spatial Type	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|
3.3 Spatial Coordinates	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|
3.4 Geographic Region Name	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|
3.5 Geographic Bounding Box - Lower Left Corner  	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|
3.6 Bounding Box - Upper Right Corner  	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|
3.7 Bounding Box - Coordinate Reference System  	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|
3.8 Geographic Bounding Box - Dimensions  	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|
3.9 Temporal coverage	|	-	|	-	|	-	|	ds:temporalCoverage	|	dcterms:temporal	|	-	|	-	|	http://data.gouv.fr/onto#dateDebut and http://data.gouv.fr/onto#dateFin	|
3.10 Temporal coverage starts	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|
3.11 Temporal coverage ends	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|
3.12 Temporal granularity	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|
3.13 Temporal granularity factor	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|
3.14 Periodicity of data(set) collection	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|
3.15 Periodicity of the production process	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|
3.16 Periodicity of the estimates	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|
3.17 Temporal and spatial comparability	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|
3.18 Periodicity of data dissemination	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|
3.19 Data quality	|	-	|	-	|	-	|	-	|	dcat:dataQuality	|	-	|	-	|	-	|
3.20 Reference period	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|
4. *Supplemental Information*	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|
4.1 Documentation URL - resource	|	-	|	-	|	-	|	-	|	dcat:dataDictionary 	|	-	|	-	|	http://data.gouv.fr/onto#RessourceAnnexe	|
5. *Distribution Information*	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|
5.1 Licence	|	-	|	-	|	-	|	-	|	dcterms:license	|	-	|	-	|	dcterms:license	|
5.2 Copyright	|	-	|	-	|	-	|	sdo:copyrightHolder	|	-	|	-	|	-	|	-	|
5.3 Size	|	-	|	-	|	-	|	sdo:contentSize	|	dcat:size	|	-	|	-	|	http://data.gouv.fr/onto#taille	|
5.4 URL - resource	|	-	|	-	|	-	|	sdo:contentUrl	|	dcat:accessURL	|	adms:accessURL	|	-	|	http://data.gouv.fr/onto#fileUpload and http://data.gouv.fr/onto#accesURL	|
5.5 Homepage URL	|	-	|	-	|	-	|	sdo:url	|	foaf:homepage	|	-	|	-	|	-	|
5.6 Format - resource	|	-	|	-	|	-	|	sdo:encodingFormat	|	dcterms:format	|	dcterms:format	|	-	|	dcterms:format	|
5.7 Language	|	-	|	-	|	-	|	sdo:inLanguage	|	dcterms:language	|	dcterms:language	|	-	|	dcterms:language	|


**Mapping**
Please find the metadata mapping index between G8 nations [here](https://github.com/nsinai/G8_Metadata_Mapping/blob/master/index.md).

**Feedback**
Please give feedback on this mapping - you can fill out a [short survey (5 questions)](http://www.surveymonkey.com/s/CCM3F2C) or a [longer survey (10 questions)](http://www.surveymonkey.com/s/N2ZMP7K).


