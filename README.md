# 2000Lakes_web
This is an interactive platform prototype for the 2000Lakes project.


### Try a demo
***Current platform has some issues with Safari. Please use Chrome or Firefox if possible.***  
To run the web locally, use python 3, type ``http-server`` in the terminal. Pleases install all the necessary dependencies.  
The web can also be accessed from this link: [https://2000lakes.github.io/2000Lakes_web/](https://2000lakes.github.io/2000Lakes_web/)


### Documents explanation
**Folder data**: necessary data for the web visualization.  
>***full_data.csv***: full data for lakes. Data from the research project and from Wikipedia are integrated in this file. It is important to have the new lakes added with the same format in this file.  
>**folder cantons**: contains seperate data for lakes in each canton. Each file is extracted from **full_data.csv**. Once the full data file is updated, this folder should be updated as well. Code for extraction is in the **data_preprocess.ipynb**.  
>**cantons.geojson**: geojson file for all cantons, downloaded form Swisstopo.    
>**tot_lake.geojson**: downloaded geojson file from Swisstopo including lakes that are not in our database.  
>**folder lakes_geojson**: seperate geojson file for each lake, named in lake id.  
>**tot_sampled.csv**: sampled data from 2000Lakes. Integrated into **full_data.csv**.   
>**data_preprocess.ipynb**: process code for the data (not used in web implementation).  
            
**Folder lib**: necessary libraries for web implementation.

**Folder node_modules**: the library canvas-confetti for visualizing the winning effect of the chatbot game.

**index.html**: main web page. To modify the main web, one way is to add more section in this file and add a seperate js file. Avoid duplicated variable names!  

**lake_page.html**: web page for lake info, generated from map.js.

**empty_wiki.html**: web page showing invitation to create Wikipedia page for lake.

**footer.html**: footer part embeded on other pages.

**bar.js**: code for the progress bar viz.

**game.js**: code for the chatbot game.

**gashapon.js**: code for the gashapon machine.

**map.js**: the main viz part, map implementation, including all interaction related to the map.

**measures.js**: code for the interactive measures.

**radioBtn.js**: code for the radio buttons in the first section.

**resizeupdate.js**: code for resizing the main elements when the window size changed.

**style.css**: the main style file. Style for new elements should be added here.
