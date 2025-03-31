---
layout: default
title: San Francisco’s Drug Crisis Through Data (2014–2024)
---
# Introduction
San Francisco’s struggle with drug-related crime over the past decade reflects a complex interplay of policy shifts, public health crises, and law enforcement priorities. Using the San Francisco Police Department Incident Report dataset (2003–2024), this analysis examines how drug/narcotic incidents evolved in response to societal and institutional changes. The dataset includes details such as crime category, date/time, police district, and latitude/longitude coordinates, providing critical insights into temporal and spatial patterns of drug-related crime.

## Policy Shifts and Their Impact

In 2014, California voters passed Proposition 47, which reclassified many non-violent drug offenses from felonies to misdemeanors. This landmark legislation aimed to reduce incarceration rates but had unintended consequences for law enforcement priorities. As shown in the time-series chart below [Figure 1](#figure1), the proportion of drug/narcotic incidents relative to total crimes began to decline after 2014 [[1]](#ref1). While this trend reflects reduced enforcement of low-level drug crimes, it does not capture the rising tide of addiction and overdose deaths during this period [[1]](#ref1).
<div style="text-align: center;">
  <a id="figure1"></a>
  <img src="plot_1.jpg" alt="Description of image" style="max-width: 100%;">
</div>
<p>
  <strong>Figure 1:</strong> A brief overview of the data trends.
</p>
By 2017, fentanyl—a synthetic opioid up to 50 times more potent than heroin—arrived in San Francisco. Its proliferation marked a turning point in the city’s drug crisis. The time-series chart reveals a sharp spike in reported drug/narcotic incidents between 2017 and 2018, coinciding with fentanyl’s emergence as a dominant force in the local drug market [[5]](#ref5). Unlike previous opioids, fentanyl’s potency led to unprecedented overdose rates, overwhelming public health systems and sparking renewed calls for action [[3]](#ref3).

## Neighborhood-Level Disparities

While fentanyl affected communities across San Francisco, its impact was most visible in neighborhoods like the Tenderloin and South of Market (SOMA). These areas have long been epicenters of homelessness and poverty, creating fertile ground for open-air drug markets. The interactive district-level visualization below [Figure 2](#bokeh1) highlights how drug-related crime became increasingly concentrated in these neighborhoods over time. By 2020, over 50% of all reported drug/narcotic incidents occurred in the Tenderloin alone—a stark reminder of systemic inequities in how addiction is policed and addressed [[4]](#ref4).

<div >
  <a id="bokeh1"></a>
  <iframe src="{{ site.baseurl }}/sf_drug_interactive.html" width="108%" height="600" frameborder="0" scrolling="no">
    Your browser does not support iframes. You can view the interactive plot <a href="{{ site.baseurl }}/sf_drug_interactive.html">here</a>.
  </iframe>
</div>
<p>
  <strong>Figure 2:</strong> Drug-related crimes in San Francisco have been heavily concentrated in the Tenderloin district throughout 2014–2024. The top 4 police districts (Tenderloin, Southern, Mission, and Northern) consistently report the majority of drug-related incidents. Please note that the graph shows relative values, absolute crime numbers can be viewed by hovering.
</p>

This geographic concentration reflects both social vulnerabilities and law enforcement strategies. In February 2025, Mayor Daniel Lurie declared a fentanyl state of emergency to address the crisis ravaging neighborhoods like the Tenderloin. The ordinance expedited funding for treatment programs and opened a stabilization center in the heart of the district to provide immediate care for individuals facing substance use crises [[6]](#ref6). Filtering the interactive visualization for Tenderloin incidents from 2022 onward reveals a sharp increase in enforcement activity as police targeted dealers operating within open-air markets [[4]](#ref4).

## Geospatial Patterns: Mapping Drug Incidents

To better understand how fentanyl reshaped San Francisco’s landscape, we turn to a heatmap of drug/narcotic incidents from 2014–2024. This visualization [Figure 3](#map1) underscores the spatial disparities highlighted earlier: red zones representing high-density areas are overwhelmingly concentrated in the Tenderloin and SOMA districts. These hotspots reflect not only law enforcement activity but also broader societal challenges tied to addiction and homelessness.

<div >
  <a id="map1"></a>
  <iframe src="{{ site.baseurl }}/heatmap.html" width="100%" height="500" frameborder="0" scrolling="no">
    Your browser does not support iframes. View the map <a href="{{ site.baseurl }}/heatmap.html">here</a>.
  </iframe>
</div>
<p>
  <strong>Figure 3:</strong> The heatmap shows drug-related incident concentrations across San Francisco, with darker red indicating higher incident density. Use the time slider to view changes from 2014 to 2024. The Tenderloin and adjacent areas consistently show the highest concentration of drug-related incidents.
</p>
The heatmap also reveals shifts over time that align with key policy changes and public health interventions:

- **After Proposition 47 (2014):** Red zones expanded slightly as open-air markets became more visible due to reduced enforcement of low-level offenses [[1]](#ref1).
- **Following fentanyl’s arrival (2017):** Hotspots intensified as overdose rates surged and public scrutiny increased [[5]](#ref5).
- **Post-2022 enforcement efforts:** Led to localized spikes in activity within targeted areas like the Tenderloin but did little to address underlying causes of addiction or overdose deaths elsewhere in the city [[6]](#ref6).

## Conclusion

San Francisco’s battle against drug-related crime is a microcosm of America’s larger struggle with addiction and public health crises. While Proposition 47 aimed to reduce incarceration rates for non-violent offenses, it inadvertently shifted focus away from addressing systemic issues tied to substance abuse. Fentanyl’s arrival exacerbated these challenges, overwhelming communities already grappling with poverty and homelessness while exposing gaps in public health infrastructure.

The visualizations presented here offer a window into how these dynamics unfolded over time and across neighborhoods:
- The time-series chart captures key policy shifts and their impact on reported incidents.
- The interactive district-level tool highlights geographic disparities in enforcement activity post-2020.
- The heatmap provides a spatial overview of hotspots linked to fentanyl’s rise.

Together, these insights underscore the need for holistic approaches that balance law enforcement priorities with investments in treatment programs, harm reduction strategies, and community support systems.

## References

1. <a id="ref1"></a> Lopez, G., Katz, J., & Parlapiano, A. (2024). *Can San Francisco Solve Its Drug Crisis? The New York Times.* [Link]( https://www.nytimes.com/2024/01/31/upshot/san-francisco-drug-crisis.html?unlocked_article_code=1.7E4.a6XJ.QIxTydwlDGAL&smid=nytcore-ios-share&referringSource=articleShare)
2. <a id="ref2"></a> Carlos, C., *CBS News* (2025). *San Francisco Mayor Signs Fentanyl State of Emergency Ordinance.* [Link](https://www.cbsnews.com/sanfrancisco/news/fentanyl-state-of-emergency-san-francisco-mayor-daniel-lurie/)
3. <a id="ref3"></a> SF Department of Public Health (2024). *Overdose Prevention Plan.* [Link](https://www.sf.gov/reports--december-2024--overdose-prevention-plan-2024)
4. <a id="ref4"></a> CNN (2023). *Drugs Are Sold Out In The Open In San Francisco's Tenderloin District.* [Link](https://edition.cnn.com/2023/09/03/us/san-francisco-tenderloin-drug-market/index.html)
5. <a id="ref5"></a> SF Chronicle (2023). *Tracking San Francisco's Drug Overdose Epidemic.* [Link](https://www.sfchronicle.com/projects/san-francisco-drug-overdose-deaths/)
6. <a id="ref6"></a> SF Mayor's Office (2025). *Mayor Lurie Signs Fentanyl State Of Emergency Ordinance.* [Link](https://www.sf.gov/mayor-lurie-supervisors-celebrate-overwhelming-vote-in-support-of-fentanyl-state-of-emergency-ordinance)



## *Contributions*

- *Leo helped with the map.*
- *Dante contributed to the Bokeh visualizations.*
- *Maija assisted in creating the first series plot.*
- *All of us collaboratively wrote the story.*