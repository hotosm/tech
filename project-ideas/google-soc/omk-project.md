# OpenMapKit

## Background
The humanitarian sector faces many challenges, all of which are amplified during emergency or crisis situations where access to information is limited, coordination is strained, and lives are at stake. Beyond the emergency phase, information for decision-making in programming can be restricted, out-of-date, scattered, or available only in unusable formats. Organizations working to support communities therefore have limited access to accurate information, which can negatively impact the people their programs are designed to support. Numerous examples can be highlighted, such as out of date census materials leading to poor targeting of beneficiary communities or limited geographic information causing failure to identify appropriate hazards and risks. This inability to accurately understand a given context  can be contributed to organizations failing to leverage technology to its full potential. Moreover, while many agencies recognize and value information collection through the use of technologies such as GIS, in practice few understand how to apply these technologies and fewer still understand how to successfully integrate them into core activities. Data collected for communities and neighbourhoods frequently remains in the hands of the organization who has conducted the assessment. Data may not even be shared within an organization, or used beyond the scope of narrowly-defined projects. Having shared, open, up-to-date geographic data available through OSM can greatly enhance the effectiveness and efficiency of disaster response for agents and responders across the humanitarian spectrum.

Opportunities to integrate geographic information to improve project management exist all along the disaster management cycle, but are frequently seen as an ad hoc or one-off activity performed during a project or response. However, leveraging geographic information alongside socio-economic survey information can deepen understanding and analysis; contribute to evidence-based decision-making; link strongly with improved information management needed to promote efficient and effective systems and well-organized responses; and further the humanitarian cause by improving community selection through increased transparency.  GIS itself also reinforces better planning processes (you need to know what you want to map and how the data is going to be used at the outset to avoid wasting resources), fosters dialogue between local actors, and collected data can create important sustainable records of assessment findings, hazard maps and improve overall risk analysis.  At a community level, utilizing technological tools to collect project data can reduce errors and delays associated with manually-linking digital survey data to GIS features—an emerging development best practice.  

An 'open data/map' app was originally conceived from OpenStreetMap (OSM) damage assessment research during the 2013 Typhoon Haiyan response on behalf of the American Red Cross and the United States Agency for International Development (USAID). Among the recommendations that came out of the assessment were the needs to have better base mapping, and for better damage and survey tools for geospatial data. In early 2014, during a competitive proposal process the American Red Cross was chosen by USAID/OFDA to build a survey tool to link OpenDataKit (ODK) and OSM as part of work tied to a project in Dhaka, Bangladesh. In June of 2014, the Humanitarian OpenStreetMap Team (HOT) was awarded a Knight Prototype Fund in order "to allow easier collection of open geographic data, even in places with connectivity issues, by combining Open Data Kit’s data collection with OpenStreetMap’s data community." The result of the collaborative funding and development efforts was OpenMapKit.

## OpenMapKit

OpenMapKit integrates with ODK to unite the collection of OSM data and private survey information. It is openly licensed under a BSD 3-Clause license, with all the code hosted on GitHub. Attributes can be added to OSM features while also collecting private survey data that can be linked to GIS features.

American Red Cross has used OpenMapKit in a variety of community mapping projects including in:

* [Riohacha, Colombia](http://www.missingmaps.org/blog/2016/03/29/riohacha-colombia/)
* [West Africa](http://www.missingmaps.org/blog/2016/04/25/west-africa-mapping-hub-launch/)
* [Binga District, Zimbabwe](http://www.missingmaps.org/blog/2016/06/07/zimbabwe/)

OpenMapKit has been used by Ramani Huria in Tanzania:

* [Mapping Dar es Salaam's Water, Sanitation and Hygiene Facilities](https://www.hotosm.org/updates/2016-10-19_mapping_dar_es_salaams_water_sanitation_and_hygiene_facilities)
* [Ramani Huria Trains Secondary Students During STEM Boot Camp](http://ramanihuria.org/ramani-huria-trains/)
* [Ramani Huria OMK Field Data Cleaning Workflow](https://wiki.openstreetmap.org/wiki/Ramani_Huria_OMK_Field_Data_Cleaning_Workflow)

CartoNG conducted a benchmarking to compare a few geographic mobile data collection tools including OpenMapKit:
http://blog.cartong.org/2017/05/05/benchmarking-mdc-tools-with-strong-gis-component/ 

Use by Humanitarian OpenStreetMap Team in:
* Indonesia
* Tanzania
* Liberia
* Uganda

Continued use of OpenMapKit has resulted in improvements to the Android app as well as the larger ecosystem such as [OpenMapKit Server](https://github.com/posm/OpenMapKitServer#openmapkit-server) and [Portable OpenStreetMap (POSM)](https://github.com/posm/posm#posm).

There are a number of desired improvements to OpenMapKit Android that have been logged by various uses as issues on the GitHub repository. Some inital scoping discussion has happened here: https://github.com/hotosm/tech/issues/98. 

## Project scope

The project would be focused on implementing two useful improvements: 

1. Change the map renderer. Shift to Mapbox Vector Tiles. Remove the need to generate and upload mbtiles files to mobile devices. 
2. Add line editing. Ability to edit polylines in OMK app, so users can split a road and add the correct name to the two seperate features on the ground
