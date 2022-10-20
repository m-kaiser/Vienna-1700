# Vienna 1700
This repository contains historical GIS Data for the mapping of the city of Vienna around the year 1700. It is based on the digitization of two historical city maps: the city maps of Arnold Steinhausen (1710) and Jacob Marinoni (1706). The so-called Steinhausenplan displays the city of Vienna and parts of its suburbs in great detail. The Marinoniplan on the other hand, shows the city and its suburbs as a whole but with less details. It was used as additional resource for mapping the complete extent of the aera and define place markers for the suburbs.
## Bringing the map sources together
The Steinhausenplan as georeferenced map is provided by the city of Vienna and can be accessed through the [Open Data Portal](open.data.gv.at). It is based on an original map held by the Wien Museum. Due to its age, some details are not recognizable. For the digital reconstruction in QGIS it was therefore necessary to use a better readable version of the original map to fill these gaps. This second version could be found in the map collection of the Austrian National Library. By georeferencing this additional map tiles, the missing parts could be added to the digital map. The map itself has been digitized on the layer of building parcels. Additional map details such as the fortification and river Danube were also added. 
For the digitization of the suburbs, the Marinoniplan was used. The original map from the Wien Museum is a little bit older than the Steinhausenplan and present similar age-related challenges. In this case, a reproduction of the map published in the *Historischer Atlas von Wien* (eng. Historical Atlas of Vienna) was used. The Marinoniplan shows mostly building blocks and some scattered stand-alone buildings in the outskirts of the suburbs. 
## Researching the addresses
The addresses mentioned in historical sources of that time can be categorized as shield or house names. Shield names were often linked to the occupation of its inhabitants ([Hasenhaus, Rabbit House](https://www.geschichtewiki.wien.gv.at/index.php?title=Hasenhaus&oldid=814378)) or stories from local history ([wo der Hahn den Hühnern predigt, where rooster is preaching to the chickens](https://www.geschichtewiki.wien.gv.at/index.php?title=Wo_der_Hahn_den_H%C3%BChnern_predigt&oldid=188609)). The house names were derived from the family name of its owner and can be found in many variant names depending on the source. For the identification of a single address, the multi-volume work of Paul Harrer-Lucienfeld *Wien. Seine Geschichte, Menschen und Kultur* was very useful. He compiled a detailed building history for the first district of Vienna based on the evaluation of land registers. By using this source, it was possible to identify the Haller’sche Haus, which was owned by the court inspector Michael Haller in the 2<sup>nd</sup> half of the 17th century, as a location on the modern address [Wollzeile 21](https://www.digital.wienbibliothek.at/Drucke/content/pageview/2289034). The coordinates for this address were then placed on the basis of the Steinhausenplan. Addressses belonging to the suburbs couldn't be identified.
# Dataset
- Steinhausenplan 1706 (map as geojson)
- Marinoniplan 1710 (map as geojson)
- Vorstädte Lat Lon (suburbs as table)
- Wohnadressen (addresses as table)

# Interactive Map
![image of interactive map](https://github.com/m-kaiser/Vienna-1700/blob/main/Vienna_1700_interactive_map_preview1.png)
> The historical GIS data was originally compiled for the visualization of prospographical data belonging to the VieCPro-project. For testing the possibilities of an interactive map, a sample of 973 persons and their 1.065 addresses (92 persons had more than one address in the sample) from the Leopold dataset was used to visualize the distribution over the city of Vienna. [Try it out!](https://m-kaiser.github.io/viecpro-wohnadressen/)
# Publications
- Maximilian Kaiser, Wo das Personal Kaiser Leopolds I. wohnte: digitale Spurensuche mittels prosopographischer Daten von VieCPro, in: Michael Portmann (Red.), Die Habsburgmonarchie. Fragen, Quellen und Ergebnisse zur Geschichte der Neuzeit, hrsg. v. Institut für die Erforschung der Habsburgermonarchie und des Balkanraumes, 28.2.2022, [https://habsmon.hypotheses.org/706](https://habsmon.hypotheses.org/706).
- Maximilian Kaiser, VieCPro Wohnadressen, in: Zenodo, v.1.0.1 (20.10.2022). [DOI: 10.5281/zenodo.7228177](https://doi.org/10.5281/zenodo.7228177)
# Sources
- Werner Arnold Steinhausen, Iosepho Augusto Ichnographiam hanc Imperialis Suae Sedis Viennae Austriae Iussu Supremi Regiminis ejùsq. Gubernatoris, Caroli Ferdinandi Sac. Rom. Imp, Comitis à Weltz Sac: Caes.ae Mtt.is Camerarij et Consiliarij intimi accuraté desumptam …, ÖNB Kartensammlung, Sign. AB 7 A 56, 1710, [http://data.onb.ac.at/rec/AC03803441](http://data.onb.ac.at/rec/AC03803441)
- Werner Arnold Steinhausen (Kartograph), Grundrissplan der Stadt Wien mit dem Glacis und angrenzenden Teilen der Vorstädte im Jahre 1710, Wien Museum, Inv.-Nr. 105500, 1710, CC0 ([https://sammlung.wienmuseum.at/objekt/783299/](https://sammlung.wienmuseum.at/objekt/783299/))
- Jacob Marinoni (Kartograph), Christian Engelbrecht (Stecher), Antonio Maria Niccolo Beduzzi (Zeichner), Leandro Anguissola (Kartograph) und Johann Andreas d. Ä. Pfeffel (Stecher), Grundrissplan von Wien mit seinen Vorstädten und dem Linienwall. 1704 mit Legende (4 Teile), 1706, Wien Museum Inv.-Nr. 105980, CC0 ([https://sammlung.wienmuseum.at/objekt/182622/](https://sammlung.wienmuseum.at/objekt/182622/))
- 5.2/1706 Wien mit Vorstädten 1706 ([Reproduktion des Plans von Leander Anguissola und Jacob Marinoni](https://www.wien.gv.at/actaproweb2/benutzung/archive.xhtml?id=Stueck++52FDBB08-0BE5-4C3F-A2FD-CA0E3324031Alanm08sch#Stueck__52FDBB08-0BE5-4C3F-A2FD-CA0E3324031Alanm08sch)), in: Felix Czeike, Ferdinand Opll und Renate Banik-Schweitzer, Historischer Atlas von Wien, 3. Lieferung, Wien: Pichler, 1987. 
- Paul Lucienfeld-Harrer, Wien. Seine Häuser, Menschen und Kultur, 19-bändig, Wien: Selbstverlag, 1951-1958. (Manuskript) [urn:nbn:at:AT-WBR-124776](https://resolver.obvsg.at/urn:nbn:at:AT-WBR-124776)
