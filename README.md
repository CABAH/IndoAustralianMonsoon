# Indo-Australian Monsoon record
A continuous, absolute-dated, 150,000-year record of monsoon hydroclimate dynamics from a permanent lagoon (<a href="https://doi.org/10.1017/qua.2020.50">Girraween</a>) in the core monsoon region of northern Australia, compared to global circulation model hindcasts
<p><a href="https://www.arc.gov.au/news-publications/media/research-highlights/getting-bottom-girraween-lagoon"><img align="bottom-left" src="www/GirraweenCoring.jpg" alt="coring on Girraween Lagoon" width="350" style="margin-bottom: 20px"></a> &nbsp; &nbsp; &nbsp; &nbsp; <img align="bottom-right" src="www/LOVECLIMspelprcpLprcpGcorL.jpg" alt="example time series" width="420" style="margin-top: 60px"></p>

Contributors: <a href="https://globalecologyflinders.com/people/#CJAB">Corey J. A. Bradshaw</a>, <a href="https://globalecologyflinders.com/people/#FS">Frédérik Saltré</a>, <a href="https://research.jcu.edu.au/portfolio/michael.bird">Michael Bird</a>

Accompanies paper:<br>
<br>
Bird, MI, M Brand, R Comley, X Hadeen, Z Jacobs, C Rowe, F Saltré, CM Wurster, C Zwart, CJA Bradshaw. A 150,000 year terrestrial record of major change in Indonesian-Australian monsoon activity. In preparation

## Abstract
Nearly two thirds of the world’s population depends on monsoon rainfall. Monsoon failure and extreme precipitation events have impacted societies for millennia, but the distribution and amount of monsoon precipitation is predicted to change with climate warming, albeit regional trajectories are uncertain. Multiple terrestrial records of east Asian monsoon variability over multiple glacial-interglacial cycles have been developed in the last decade, but there are no terrestrial records of equivalent length of the coupled Indo-Australian monsoon towards the southern monsoon limit — the Australian continent. Here we present a continuous, absolute-dated, 150,000-year record of monsoon hydroclimate dynamics from a permanent lagoon in the core monsoon region of northern Australia. We show that Australian rainfall is broadly anti-phased with the East Asian monsoon. We identify periods of intense monsoon activity associated with high local insolation in Marine Isotope Stage 5 during known ‘megalake’ phases in the arid interior of Australia. We also identify periods of monsoon intensification unrelated to insolation maxima, but associated with Heinrich events coincident with weak monsoon events in East Asia. The results suggest that strong asymmetry in inter-hemispheric monsoon rainfall  might accompany any weakening in the strength of the Atlantic meridional overturning circulation resulting from future climate change. This asymmetry will involve drying in the heavily populated monsoon domain of the Northern Hemisphere and intensification of rainfall in the Southern Hemisphere.

## <a href="https://github.com/cjabradshaw/IndoAustralianMoonsoon/tree/main/scripts">Scripts</a>
- <a href="https://github.com/cjabradshaw/IndoAustralianMoonsoon/blob/main/scripts/GirraweenMonsoonGithub.R"><code>GirraweenMonsoonGithub.R</code></a>

## <a href="https://github.com/cjabradshaw/IndoAustralianMoonsoon/tree/main/data">Data</a>
- <em>ChSpeleo2.csv</em>: China <a href="https://doi.org/10.1029/2011GL050202">speleothem</a> record (<sup>18</sup>O)
- <em>LOVECLIM_NTRegionClimate(1-150ka)_anomalies(Precipitation).csv</em>: <a href="https://gmd.copernicus.org/articles/3/603/2010/">LOVECLIM</a> global circulation model hindcasts of precipitation anomalies for northern Australia
- <em>LOVECLIM_SARegionClimate(1-150ka)_anomalies(Precipitation).csv</em>: LOVECLIM global circulation model hindcasts of precipitation anomalies for South Asia
- <em>LOVECLIM_Gironly(1-150ka)_anomalies(Precip).csv</em>: LOVECLIM global circulation model hindcasts of precipitation anomalies for the <a href="https://doi.org/10.1017/qua.2020.50">Girraween</a> cell
- <em>rainLoveClGWdistcor2.csv</em>: distance-to-coast-corrected rainfall at Girraween from the LOVECLIM global circulation model hindcasts
- <em>NTRegionClimate(0-150ka)_anomalies(Precipitation)</em>: <a href="https://www.metoffice.gov.uk/research/approach/modelling-systems/unified-model/climate-models/hadcm3">Hadley Centre Coupled Model version 3</a> (HadCM3) global circulation model hindcasts of precipitation anomalies for northern Australia
- <em>HadCM3_Gironly(0-150ka)_anomalies(Precip).csv</em>: Hadley Centre Coupled Model version 3 (HadCM3) global circulation model hindcasts of precipitation anomalies for the <a href="https://doi.org/10.1017/qua.2020.50">Girraween</a> cell
- <em>HADCMS rel rainfall.csv</em>: distance-to-coast-corrected rainfall at Girraween from Hadley Centre Coupled Model version 3 (HadCM3) hindcasts
- <em>rainrel.csv</em>: a test corrected rainfall dataset (redacted)
- <em>Hiso.csv</em>: hydrogen isotope (<a href="https://doi.org/10.1017/qua.2020.50">Girraween</a> core)
- <em>dole2.csv</em>: <a href="https://link.springer.com/referenceworkentry/10.1007/978-1-4020-4411-3_71">Dole effect</a> ΔDE* ‰
- <em>insol.csv</em>: <a href="https://www.sciencedirect.com/topics/earth-and-planetary-sciences/insolation">insolation</a> W m<sup>-2</sup>
- <em>toc.csv</em>: % total organic carbon (<a href="https://doi.org/10.1017/qua.2020.50">Girraween</a> core)
- <em>tree.csv</em>: % tree pollen (<a href="https://doi.org/10.1017/qua.2020.50">Girraween</a> core)

## R libraries
- <code>spatstat</code>, <code>gstat</code>, <code>maps</code>, <code>sp</code>, <code>ape</code>, <code>permute</code>, <code>ggplot2</code>, <code>dplyr</code>, <code>boot</code>
<code>tmvnsim</code>, <code>wCorr</code>, <code>truncnorm</code>, <code>orcutt</code>, <code>lmtest</code>

<p><a href="https://www.flinders.edu.au"><img align="bottom-left" src="www/Flinders_University_Logo_Horizontal_RGB_Master.png" alt="Flinders University logo" width="160" style="margin-top: 20px"></a>  &nbsp; &nbsp;
<a href="https://globalecologyflinders.com"><img align="bottom-left" src="www/GEL Logo Kaurna New Transp.png" alt="GEL logo" width="80" style="margin-top: 20px"></a>  &nbsp; &nbsp;
 <a href="https://EpicAustralia.org.au"><img align="bottom-left" src="www/CabahFCL.jpg" alt="CABAH logo" width="200" style="margin-top: 20px"></a>  &nbsp; &nbsp; <a href="https://www.jcu.edu.au"><img align="bottom-left" src="www/jculogo.png" alt="JCU logo" width="70" style="margin-top: 20px"></a></a></p>

