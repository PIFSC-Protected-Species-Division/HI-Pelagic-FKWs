<!-- README.md is generated from README.Rmd. Please edit that file -->

# Developing a management area for Hawaiʻi pelagic false killer whales

This repository contains files referenced in Oleson et al. (2023) that
pertain to the development of a new management area for the Hawaiʻi
pelagic stock of false killer whales. The first files, located in the
[data](https://github.com/PIFSC-Protected-Species-Division/HI-Pelagic-FKWs/tree/main/data)
folder, summarize the available biological data for Hawaiʻi pelagic
false killer whales, including the genetic sample, survey sighting, and
fishery interaction data. The metadata for these files are detailed
below. Each of the three data files can be downloaded by clicking on the
file of interest within the
[data](https://github.com/PIFSC-Protected-Species-Division/HI-Pelagic-FKWs/tree/main/data)
folder and then clicking on the “download raw file” button to the upper
right of the file preview. Note that the satellite telemetry data also
used to develop the new management area is available from the [Animal
Telemetry network](https://portal.atn.ioos.us/#metadata/137104/species).

The remaining files, located in the
[boundary](https://github.com/PIFSC-Protected-Species-Division/HI-Pelagic-FKWs/tree/main/boundary)
folder, comprise a shapefile of the new Hawaiʻi pelagic false killer
whale management area. The shapefile contains a line feature with a
current projection of WGS_1984_UTM_Zone_4N. The shapefile was created by
Amanda Bradford at the NOAA Fisheries Pacific Islands Fisheries Science
Center using the satellite telemetry, genetic sample, survey sighting,
and fishery interaction data as described in Oleson et al. (2023). For
ease and simplicity, metadata for the shapefile were entered using the
“Item Description” style in ArcGIS Desktop, but this may be updated in
the future.

Downloading individual components of a shapefile is not recommended;
however, downloading individual folders from GitHub is not intuitive.
The easiest way to obtain the management area boundary is to download
the repository by clicking on the green “Code” button in the upper right
of this page and selecting “Download ZIP”. You can then delete the files
and folders you do not need. If you have any questions or issues with
any of the files, please contact Amanda Bradford at
amanda.bradford@noaa.gov.

## Genetic sample data

Sample locations of false killer whales within the central North Pacific
(defined as the area from the equator to 43°N, and from 175°E to 132°W)
were compiled for use in defining the Hawaiʻi pelagic false killer whale
management area. All processed samples collected to date (i.e., through
17 April 2021) were included, excluding those from the main Hawaiian
Islands insular and Northwestern Hawaiian Islands stocks. The resulting
file “01_pFKW_GenSamps_CNP_1997-2021.csv” contains the following
information:

| Column heading | Explanation                                                                                                                                                                                                            |
|----------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Date           | Date of sample collection (m/d/yyyy)                                                                                                                                                                                   |
| LabID          | Lab identification number assigned by the NOAA Fisheries Southwest Fisheries Science Center Marine Mammal Genetics Program                                                                                             |
| Duplicate      | Lab identification number of the sample taken from the same individual                                                                                                                                                 |
| FieldID        | Identification label associated with the sample source; longline fishery trip numbers have been obscured to maintain confidentiality                                                                                   |
| Sex            | Sex of the individual, either female (F), male (M), or unknown (U)                                                                                                                                                     |
| Haplotype      | Pelagic haplotype number; the unknown (U) number represents a case where a single ambiguous base during sequencing prevented assignment, and “New” refers to a new haplotype that is in the process of being confirmed |
| Lat            | Latitude of sample location in decimal degrees                                                                                                                                                                         |
| Lon            | Longitude of sample location in decimal degrees                                                                                                                                                                        |
| InMgmtArea     | Sample location is within (TRUE) or outside (FALSE) the new management area                                                                                                                                            |

## Survey sighting data

Sightings of false killer whales during NOAA Fisheries ship-based
line-transect surveys of the central North Pacific were extracted to
help guide the definition of the the Hawaiʻi pelagic false killer whale
management area. All sightings made to date (i.e., through 3 March 2020)
were included, excluding those of the main Hawaiian Islands insular and
Northwestern Hawaiian Islands stocks. The resulting file
“02_pFKW_SurSights_CNP_1986-2020.csv” contains the following
information:

| Column heading | Explanation                                                                                                                                                                                                                                                                                                               |
|----------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Date           | Date of survey sighting (m/d/yyyy)                                                                                                                                                                                                                                                                                        |
| SurveyNo       | Survey number assigned by NOAA Fisheries                                                                                                                                                                                                                                                                                  |
| Ship           | Survey vessel (three-letter abbreviation, email amanda.bradford@noaa.gov for full ship name)                                                                                                                                                                                                                              |
| SightNo        | Sighting number assigned during survey                                                                                                                                                                                                                                                                                    |
| Time           | Local time of sighting                                                                                                                                                                                                                                                                                                    |
| Effort         | Sighting was made while ON or OFF effort                                                                                                                                                                                                                                                                                  |
| EffType        | Sighting was made while on systematic (S), non-systematic (N), or fine-scale effort or while off-effort (O)                                                                                                                                                                                                               |
| Mixed          | Sighting was of mixed-species (TRUE) or only of false killer whales (FALSE)                                                                                                                                                                                                                                               |
| Lat            | Latitude of sighting location in decimal degrees                                                                                                                                                                                                                                                                          |
| Lon            | Longitude of sighting location in decimal degrees                                                                                                                                                                                                                                                                         |
| Biopsy         | Genetic sample(s) collected (Yes) or not (No) during sighting                                                                                                                                                                                                                                                             |
| Photos         | Photos collected (Yes) or not (No) during sighting                                                                                                                                                                                                                                                                        |
| Tag            | Satellite tag(s) deployed (Yes) or not (No) during sighting                                                                                                                                                                                                                                                               |
| stockArea      | Stock area of sighting location, either within the U.S. EEZ around the Hawaiian Islands (HawaiiEEZ) or Palmyra (PalmyraEEZ), within the boundary of the main Hawaiian Islands (MHI) insular or Northwestern Hawaiian Islands (NWHI) stocks or the overlap between the two (MHI-NWHI), or outside the U.S EEZ (OutsideEEZ) |
| InMgmtArea     | Sighting location is within (TRUE) or outside (FALSE) the new management area                                                                                                                                                                                                                                             |
| Stock          | Stock assignment from genetic, photo, tag, or locality inference, either Hawaiʻi pelagic (HIPelagic), Palmyra, or unknown pelagic (UnkPelagic), with sightings that could be of either the Hawaiʻi pelagic, MHI, or NWHI stocks represented accordingly (MHIorHIPelagic, NWHIorHIPelagic, or MHIorNWHIorHIPelagic)        |

## Fishery interaction data

All false killer whale interactions with the Hawaiʻi-based longline
fisheries were aggregated to inform defining the Hawaiʻi pelagic false
killer whale management area. All interactions from 2001 through 2022
were included. The resulting file “03_pFKW_FishTakes_All_2001-2022.csv”
contains the following information:

| Column heading | Explanation                                                                                                                                                                                                                                                                                                 |
|----------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Date           | Date of fishery interaction (m/d/yyyy)                                                                                                                                                                                                                                                                      |
| TripArrYear    | Year the fishing trip arrived to port                                                                                                                                                                                                                                                                       |
| Fishery        | Hawaiʻi-based longline fishery, either deep-set (DS) or shallow-set (SS), with tuna-targeting deep sets (T) applied to 2001 prior to a regulatory change                                                                                                                                                    |
| Lat            | Latitude of interaction location in decimal degrees                                                                                                                                                                                                                                                         |
| Lon            | Longitude of interaction location in decimal degrees                                                                                                                                                                                                                                                        |
| stockArea      | Stock area of interaction location, either within the U.S. EEZ around the Hawaiian Islands (HawaiiEEZ), Palmyra (PalmyraEEZ), or Johnston (JohnstonEEZ); within the boundary of the main Hawaiian Islands (MHI) insular or Northwestern Hawaiian Islands (NWHI) stocks; or outside the U.S EEZ (OutsideEEZ) |
| InMgmtArea     | Interaction location is within (TRUE) or outside (FALSE) the new management area                                                                                                                                                                                                                            |
| Stock          | Stock assignment from genetic or locality inference, either Hawaiʻi pelagic (HIPelagic), Palmyra, or unknown pelagic (UnkPelagic), with interaction that could be with either the Hawaiʻi pelagic, MHI, or NWHI stocks represented accordingly (MHIorHIPelagic or NWHIorHIPelagic)                          |
| InjDet         | Severity of injury resulting from interaction, either serious, non-serious, cannot-be-determined (CBD), or dead following NOAA Fisheries injury determination [guidelines](https://www.fisheries.noaa.gov/action/revisions-process-distinguishing-serious-non-serious-injury-marine-mammals)                |
| Biopsy         | Genetic sample collected (Yes) or not (No) during interaction                                                                                                                                                                                                                                               |

### Disclaimer and License

<sub>This repository is a scientific product and is not official
communication of the National Oceanic and Atmospheric Administration, or
the United States Department of Commerce. All NOAA GitHub project
content is provided on an ‘as is’ basis and the user assumes
responsibility for its use. Any claims against the Department of
Commerce or Department of Commerce bureaus stemming from the use of this
GitHub project will be governed by all applicable Federal law. Any
reference to specific commercial products, processes, or services by
service mark, trademark, manufacturer, or otherwise, does not constitute
or imply their endorsement, recommendation or favoring by the Department
of Commerce. The Department of Commerce seal and logo, or the seal and
logo of a DOC bureau, shall not be used in any manner to imply
endorsement of any commercial product or activity by DOC or the United
States Government.

<sub>This content was created by U.S. Government employees as part of
their official duties. This content is not subject to copyright in the
United States (17 U.S.C. §105) and is in the public domain within the
United States of America. Additionally, copyright is waived worldwide
through the CC0 1.0 Universal public domain dedication.

<img src="https://raw.githubusercontent.com/nmfs-general-modeling-tools/nmfspalette/main/man/figures/noaa-fisheries-rgb-2line-horizontal-small.png" alt="NOAA Fisheries" height="75"/>

[U.S. Department of Commerce](https://www.commerce.gov/) \| [National
Oceanographic and Atmospheric Administration](https://www.noaa.gov) \|
[NOAA Fisheries](https://www.fisheries.noaa.gov/)
