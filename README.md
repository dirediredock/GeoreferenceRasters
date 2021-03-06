# GeoreferenceRasters

Shared here is small part of my PhD project funded by a Mitacs fellowship at the Global Ocean Modelling Lab (GOM) of The University of British Columbia (UBC), in partnership with Tsleil-Waututh Nation (TWN) and engineering consultants Kerr Wood Leidal Associates (KWL), and part of TWN’s Cumulative Effects Monitoring Initiative (CEMI). Using old raster maps and georeferencing techniques, this repo hosts the methods to reconstruct the pre-contact state of Tseil-Waut Inlet (known today as Burrard Inlet), the main waterway of Vancouver Harbour, Canada's largest and busiest port. With the completed reconstruction I discovered a 45% decrease in intertidal habitat due to Metro Vancouver's urban and port growth over the past 150 years.

<img src="https://raw.githubusercontent.com/dirediredock/GeoreferenceRasters/main/figuresGitHub/IntertidalLoss.jpg" width="100%">

The figure above shows Metro Vancouver's intertidal zone in the Inner Harbour region as it is in 2020 (blue, present state) and the reconstructed pre-urban state circa 1880 (red, proxy for the pre-contact state).

## Fine-tuning error with Function_ControlPointReticle

<img src="https://raw.githubusercontent.com/dirediredock/GeoreferenceRasters/main/figuresGitHub/ControlPointReticle.jpg" width="100%">

<img src="https://raw.githubusercontent.com/dirediredock/GeoreferenceRasters/main/figuresGitHub/PanelA.gif" width="100%">
<img src="https://raw.githubusercontent.com/dirediredock/GeoreferenceRasters/main/figuresGitHub/PanelB.gif" width="100%">
<img src="https://raw.githubusercontent.com/dirediredock/GeoreferenceRasters/main/figuresGitHub/PanelC.gif" width="100%">
<img src="https://raw.githubusercontent.com/dirediredock/GeoreferenceRasters/main/figuresGitHub/PanelD.gif" width="100%">
<img src="https://raw.githubusercontent.com/dirediredock/GeoreferenceRasters/main/figuresGitHub/PanelE.gif" width="100%">

The script `PartOne_VectorizeRasters.m` converts cropped rasters of the original [PanelA](https://github.com/dirediredock/GeoreferenceRasters/blob/main/RasterData/Originals/PanelA.jpg), [PanelB](https://github.com/dirediredock/GeoreferenceRasters/blob/main/RasterData/Originals/PanelB.jpg), [PanelC](https://github.com/dirediredock/GeoreferenceRasters/blob/main/RasterData/Originals/PanelC.jpg), [PanelD](https://github.com/dirediredock/GeoreferenceRasters/blob/main/RasterData/Originals/PanelD.jpg), and [PanelE](https://github.com/dirediredock/GeoreferenceRasters/blob/main/RasterData/Originals/PanelE.jpg) into vector point clouds in XY tall format. The figures above are the output of `PartTwo_Georeferencing.m` which uses control points to translate the maps from raster coordinates to WGS84 geospatial decimal format.

## Final run and mosaic

<img src="https://raw.githubusercontent.com/dirediredock/GeoreferenceRasters/main/figuresGitHub/allPanels.gif" width="100%">
<img src="https://raw.githubusercontent.com/dirediredock/GeoreferenceRasters/main/figuresGitHub/Mosaic.png" width="100%">

<br>

## Acknowledgement

Many thanks for the support and guidance of my supervisory committee; professor Villy Christensen (UBC, GOM), Spencer Taft (TWN, CEMI project lead), Patrick Lilley (KWL, CEMI), and colleagues Meaghan Efford (GOM, CEMI) and Greig Oldford (GOM). Special thanks to Jesse Morin (UBC, CEMI), Michelle George (TWN), and Michael George (TWN) for sharing their knowledge of Tsleil-Waut’s historical changes, Evan Thornberry (UBC) for sharing geospatial archives, and Bruce Macdonald, author of ‘Vancouver: A Visual History’ for his support and for trailblazing the historical landscape reconstruction of the region. This project unfolded through remote work between April 2020 and April 2021 at Musqueam, Squamish, Tsleil-Waututh, and Sto:lo unceded territories of Canada, and Mapuche, Kaweskar, and Selk'nam lands of Chile.

<br>


