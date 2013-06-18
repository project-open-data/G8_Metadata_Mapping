####United Kingdom Metadata

**Where to Find Data**

Where to find: The UK uses the [data.gov.uk](http://www.data.gov.uk) as a central portal for public data.

Licensing: [Open Government Licence](http://www.nationalarchives.gov.uk/doc/open-government-licence/)

Contact: http://data.gov.uk/contact

Portal API: http://data.gov.uk/data/api

**Metadata Details**

Concept|Description|Front-end (human-readable)|National metadata schema|Back-end machine-readable|Required|Data Type|Format: pattern|Cardinality|Usage Notes
------- | -------- | ----- | ---- | ---------- | ---------|-------|-------|-------|------
1. *Contact information*  |  -  |    -	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|
1.1 Person	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|
1.2 Contact Email - Publisher	|	Contact point's email address and phone number	|	Email / phone	|	-	|	Package.contact-email / contact-phone	|	No	|	string	|	-	|	-	|	-	|
1.2 Contact Email - Dataset	|	Contact point's email address and phone number	|	Email / phone	|	-	|	Group.contact-email / contact-phone	|	No	|	string	|	-	|	-	|	-	|
1.3 Organisation (Owner)	|	The contact point for the dataset or publisher.	|	Enquiries / FOI Contact	|	-	|	Package.contact-name / Package.foi-name / Group.contact-name / Group.foi-name	|	No	|	string	|	-	|	-	|	-	|
1.4 Publisher	|	The organisation closest associated with the dataset – usually the publisher, but sometimes the owner / provider.	|	Publisher	|	-	|	Group	|	Yes	|	-	|	-	|	-	|	-	|
1.5 Author	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|
1.6 Author Email	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|
1.7 Maintainer	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|
1.8 Maintainer Email	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|
2. *Dataset Identification*	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|
2.1 Unique Identifier	|	A unique identifier for the dataset	|	URI	|	-	|	name	|	Yes	|	string	|	-	|	-	|	-	|
2.2 Release Date	|	Date the metadata was added to data.gov.uk	|	Added to data.gov.uk	|	-	|	metadata_created	|	Automated	|	ISO date string	|	-	|	-	|	-	|
2.2.R Release Date	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|
2.3 Modified	|	Date changes were last made to the data.gov.uk metadata	|	Modified on data.gov.uk	|	-	|	metadata_modified	|	Automated	|	ISO date string	|	-	|	-	|	-	|
2.3.R Modified	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|
2.4 Last Updated	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|
2.4.R Last Updated	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|
2.5 Description	|	Human-readable description (e.g., an abstract) with sufficient detail to enable a user to quickly understand whether the asset is of interest.	|	Description	|	-	|	notes	|	Yes	|	markdown string	|	-	|	-	|	-	|
2.6 Keyword	|	Key words or phrases that the dataset may well have in common with other datasets, to aid navigation.	|	Tags	|	-	|	PackageTag	|	No	|	comma separated string	|	-	|	-	|	-	|
2.7 Frequency of Update	|	Frequency with which dataset is published.	|	Frequency of update	|	-	|	 frequency-of-update (UKLP only)	|	No	|	string	|	-	|	-	|	-	|
2.8 Title	|	Name given to the dataset to identify it and briefly describe it	|	Title	|	-	|	title	|	Yes	|	string	|	-	|	-	|	-	|
2.9 Category	|	Main thematic category of the dataset.	|	National Statistics	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|
3. *Extent*	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|
3.1 Spatial coverage	|	Location bounding box for which the data is relevant.	|	Dataset Extent	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|
3.2 Spatial Type	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|
3.3 Spatial Coordinates	|	-	|	Dataset Extent	|	-	|	spatial	|	No	|	GeoJSON string	|	-	|	-	|	-	|
3.4 Geographic Region Name	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|
3.5 Geographic Bounding Box - Lower Left Corner  	|	-	|	Latitude / Longitude	|	-	|	bbox-west-long, bbox-south-lat	|	No	|	float	|	-	|	-	|	-	|
3.6 Bounding Box - Upper Right Corner  	|	-	|	Latitude / Longitude	|	-	|	bbox-east-long, bbox-north-lat	|	No	|	float	|	-	|	-	|	-	|
3.7 Bounding Box - Coordinate Reference System  	|	-	|	Spatial reference system	|	-	|	spatial-reference-system	|	No	|	string	|	-	|	-	|	-	|
3.8 Geographic Bounding Box - Dimensions  	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|
3.9 Temporal coverage	|	The period of time for which the data is relevant.	|	Temporal coverage	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|
3.10 Temporal coverage starts	|	-	|	-	|	-	|	 temporal_coverage-from	|	No	|	ISO date string	|	-	|	-	|	-	|
3.11 Temporal coverage ends	|	-	|	-	|	-	|	 temporal_coverage-to	|	No	|	ISO date string	|	-	|	-	|	-	|
3.12 Temporal granularity	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|
3.13 Temporal granularity factor	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|
3.14 Periodicity of data(set) collection	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|
3.15 Periodicity of the production process	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|
3.16 Periodicity of the estimates	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|
3.17 Temporal and spatial comparability	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|
3.18 Periodicity of data dissemination	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|
3.19 Data quality	|	Datasets are graded against Tim Berners Lee's Five Stars of Openness to give a rough indication of how open they are (as described on data.gov.uk), which is related to Data quality.	|	Openness score	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|
3.20 Reference period	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|
4. *Supplemental Information*	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|
4.1 Documentation URL - resource	|	Related documents such as technical information about a dataset, developer documentation, etc.	|	Additional Resources	|	-	|	Resource.description, Resource.url, Resource.format	|	-	|	string	|	-	|	-	|	-	|
5. *Distribution Information*	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|
5.1 Licence	|	The usage licence given to the dataset, giving rights beyond those protected in Copyright and the (UK) Database Right.	|	Licence	|	-	|	license_id	|	Yes	|	string code	|	-	|	-	|	-	|
5.2 Copyright	|	(Data is assumed it is Crown Copyright)	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|
5.3 Size	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|
5.4 URL - resource	|	URL providing direct access to the downloadable distribution of a dataset.	|	URL	|	-	|	Resource.url	|	Yes	|	string	|	-	|	-	|	-	|
5.5 Homepage URL	|	Alternative landing page used to redirect user to a contextual, Agency-hosted “homepage” for the Dataset or API when selecting this resource from the Data.gov user interface.	|	Home	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|
5.6 Format - resource	|	The file format or API type of the distribution.	|	Format	|	-	|	Resource.format	|	Yes	|	string	|	-	|	-	|	-	|
5.7 Language	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|	-	|




