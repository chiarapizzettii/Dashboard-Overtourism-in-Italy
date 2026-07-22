# Overtourism in Italy
 
Interactive **R Shiny** dashboard to visualize overtourism at the province level in Italy.

https://chiarapizzetti.shinyapps.io/Overtourism_Italy/
 
## App structure (Shiny)
 
The app follows the classic three-file structure:
 
- **`global.R`** – Loads the data (shapefile and final dataset) and required libraries, run once at startup.
- **`server.R`** – App logic: reactive functions, calculations and data processing that feed the charts and the map.
- **`ui.R`** – Graphical interface: layout, filters, map and charts shown to the user.
The three files work together and the app is run via `runApp()` from the project folder.
 
## Data used
 
- `ProvCM01012026_g_WGS84.shp/.dbf/.shx/.prj` – Shapefile of Italian province boundaries (WGS84 projection).
- `final dataset.xlsx` – Dataset with overtourism indicators by province.
- 
## How to run the app
 

`library(shiny)`
`runApp()`
 
Make sure all files (\`global.R\`, \`server.R\`, \`ui.R\`, shapefile and dataset) are in the same folder.
