---
title: Safety assessment on Roslagsbanan Rail System, 2021-2022
keywords:
- Railroad Systems
- Transportation Safety
- Track Degradation
lang: en-US
date-meta: '2022-09-23'
author-meta:
- Cecilia Karina Volpe Baridon
- Elie Roudiere
- Berkan Usta
header-includes: |-
  <!--
  Manubot generated metadata rendered from header-includes-template.html.
  Suggest improvements at https://github.com/manubot/manubot/blob/main/manubot/process/header-includes-template.html
  -->
  <meta name="dc.format" content="text/html" />
  <meta name="dc.title" content="Safety assessment on Roslagsbanan Rail System, 2021-2022" />
  <meta name="citation_title" content="Safety assessment on Roslagsbanan Rail System, 2021-2022" />
  <meta property="og:title" content="Safety assessment on Roslagsbanan Rail System, 2021-2022" />
  <meta property="twitter:title" content="Safety assessment on Roslagsbanan Rail System, 2021-2022" />
  <meta name="dc.date" content="2022-09-23" />
  <meta name="citation_publication_date" content="2022-09-23" />
  <meta name="dc.language" content="en-US" />
  <meta name="citation_language" content="en-US" />
  <meta name="dc.relation.ispartof" content="Manubot" />
  <meta name="dc.publisher" content="Manubot" />
  <meta name="citation_journal_title" content="Manubot" />
  <meta name="citation_technical_report_institution" content="Manubot" />
  <meta name="citation_author" content="Cecilia Karina Volpe Baridon" />
  <meta name="citation_author" content="Elie Roudiere" />
  <meta name="citation_author_institution" content="Railway Group, KTH Royal Institute of Technology - Stockholm, Sweden" />
  <meta name="citation_author" content="Berkan Usta" />
  <link rel="canonical" href="https://uiceds.github.io/cee-492-term-project-fall-2022-time/" />
  <meta property="og:url" content="https://uiceds.github.io/cee-492-term-project-fall-2022-time/" />
  <meta property="twitter:url" content="https://uiceds.github.io/cee-492-term-project-fall-2022-time/" />
  <meta name="citation_fulltext_html_url" content="https://uiceds.github.io/cee-492-term-project-fall-2022-time/" />
  <meta name="citation_pdf_url" content="https://uiceds.github.io/cee-492-term-project-fall-2022-time/manuscript.pdf" />
  <link rel="alternate" type="application/pdf" href="https://uiceds.github.io/cee-492-term-project-fall-2022-time/manuscript.pdf" />
  <link rel="alternate" type="text/html" href="https://uiceds.github.io/cee-492-term-project-fall-2022-time/v/d106b66fc1e57aaec173513f9ceb4c32c2ee3f3f/" />
  <meta name="manubot_html_url_versioned" content="https://uiceds.github.io/cee-492-term-project-fall-2022-time/v/d106b66fc1e57aaec173513f9ceb4c32c2ee3f3f/" />
  <meta name="manubot_pdf_url_versioned" content="https://uiceds.github.io/cee-492-term-project-fall-2022-time/v/d106b66fc1e57aaec173513f9ceb4c32c2ee3f3f/manuscript.pdf" />
  <meta property="og:type" content="article" />
  <meta property="twitter:card" content="summary_large_image" />
  <link rel="icon" type="image/png" sizes="192x192" href="https://manubot.org/favicon-192x192.png" />
  <link rel="mask-icon" href="https://manubot.org/safari-pinned-tab.svg" color="#ad1457" />
  <meta name="theme-color" content="#ad1457" />
  <!-- end Manubot generated metadata -->
bibliography:
- content/manual-references.json
manubot-output-bibliography: output/references.json
manubot-output-citekeys: output/citations.tsv
manubot-requests-cache-path: ci/cache/requests-cache
manubot-clear-requests-cache: false
...






<small><em>
This manuscript
([permalink](https://uiceds.github.io/cee-492-term-project-fall-2022-time/v/d106b66fc1e57aaec173513f9ceb4c32c2ee3f3f/))
was automatically generated
from [uiceds/cee-492-term-project-fall-2022-time@d106b66](https://github.com/uiceds/cee-492-term-project-fall-2022-time/tree/d106b66fc1e57aaec173513f9ceb4c32c2ee3f3f)
on September 23, 2022.
</em></small>

## Authors



+ **Cecilia Karina Volpe Baridon**<br>
    · ![GitHub icon](images/github.svg){.inline_icon}
    [cvolpebaridon](https://github.com/cvolpebaridon)<br>
  <small>
  </small>

+ **Elie Roudiere**<br>
    · ![GitHub icon](images/github.svg){.inline_icon}
    [elieroudiere](https://github.com/elieroudiere)<br>
  <small>
     Railway Group, KTH Royal Institute of Technology - Stockholm, Sweden
  </small>

+ **Berkan Usta**<br>
    · ![GitHub icon](images/github.svg){.inline_icon}
    [berkanusta](https://github.com/berkanusta)<br>
  <small>
  </small>



# Dataset Decription
The Roslagsbanan is a railway system operating in Stockholm. As part of an improvement in the transportation system, Stockholm Municipality invested in a new fleet of trains switching from X10p trains to the new X15p. In order to analyze the safety of the new trains, brake tests were conducted. During those test runs the Latronix Track Measurement (LTM) system was mounted on the train. The LTM uses laser beams and an on-board computer to perform measurements over railroad track while the train drives on the track at normal speed. 

The data that will be used in this study was collected using the LTM system affixed to a Roslagsbanan vehicle. While the train was running over the sections, the level of each rail, alignment, curvature, cant, gauge and twist were measured every 256mm. The data was compiled in csv files and was collected between October 2021 and May 2022 with an approximate interval of one month. In other words, a given section of track typically has around six measurement files. The total amount of data is 60 CSV files of 30,000 to 80,000 rows each, for a total of 1.5GB of data. 

*These data and measurements are property of Latronix AB of Sweden, and are used with their permission for research and educational purposes only.*

In the CSV files the structure of columns is as follows:

- Marker and Marker_Offset: The kilometre post of the data point, where Marker is in km and Marker_offset is in m. In other words, if Marker=20 and MArker_offset=250.5, the kilometre post is 20,250.5 

- Coordinate_northing,Coordinate_easting, Latitude, Longitude: As their name suggests, they are the coordinates of the data point in northings and eastings, as well as latittude and longitude. 

- Speed: records the speed in km/h at which the measurement was taken. This is especially relevant as different operating speeds give different tolerances in terms of the measured properties. 

- Level_left and Level_right D0, D1, D2, D3: The deviation of the longitudinal level (height) of the left and right rail in mm, compared to its reference position. D0, D1, D2, D3 correspond to different measurement wavelengths of the same data.

- Alignment_left and Alignment_right D0, D1, D2, D3: The deviation in longitudinal alignment ("straightness")of the left and right rail in mm, compared to its reference position. D0, D1, D2, D3 correspond to different measurement wavelengths of the same data.

- Track_gauge: The deviation in the spacing between the rails in mm, from a reference of 891mm.

- Curvature: The curvature of the track at that location, in m^-1.

- Cant: The cant (inclination) of the track at the location, in mm from the horizontal.

- Twist_3m, Twist_6m: The rate of change in cant over a 3m or 6m distance.

- Level_versine_left_5m, Level_versine_right_5m: Derived from Level_left and Level_right, this level deviation in mm corresponds to longitudinal versine measurement of the top of rail over a 5m distance. This historical metric is more commonly used in railway engineering and is thus provided.

- Alignment_versine_left_10m, Alignment_versine_right_10m: Similarly to the versine level, this measure of alignment in mm uses versines over a 10m distance.

Finally, Track_name, Track_class, Station_flag and Link_name,Pos_unfiltered	Pos_filtered	NTP_sync, Cant_D1, Std_level, Std_alignment, Std_cant, Quality_1 are mainly for internal use and not part of the analysis.
			
# Project proposal
The main goal of this project is to identify patterns in the data, especially the track degradation of certain sections, and thus to analyze the change in railway safety during this time. A first approach will be to define degradation trends, and build a model to process the data that finds them automatically. Then, the study will attempt to find external factors which caused the observed trends. The analysis will include graphics of the parameters over time as well as comparing them over the sections to provide a better understanding of the data visually.

This research will help assess system performance, identify possible maintenance schedules, and provide useful data for further research in this area. The study also falls within the scope of developing predicitve maintenance in civil engineering and railways. Creating and improving analysis and predictive maintenance models such as this one can contribute to an increased safety of rail networks and a higher quality of service for passengers, They will benefit from fewer impromptu interruptions of service due to track maintenance, or even unsafe track causing line closures. 