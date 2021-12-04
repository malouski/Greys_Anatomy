---
title: "The network"
weight: 2
header_menu: true
plotly: true
---

The network of Grey's Anatomy currently consists of

2137
: nodes

9662
: edges

but the series is going strong on its 18th season (*!!!* ), so new characters are added to the wiki every week.

Since there are a lot of different characters in the series, we've divided them into 5 groups.

![static network](images/count.png)

It's not surprising that there are most patients, since new patients arrive in each episode whereas the hospital staff is more persistent.

Each character is described by their name, condition (alive or deceased) and role. Furthermore, the characters are connect to each other by having a doctor/patient relationship, being romantically involved and being family members. Let's take a look at Meredith's attributes.

name
: Meredith Grey

condition
: Alive

role
: Attending

family
: Lexie Grey, Scout Derek Shepherd Lincoln, Nancy Shepherd, Liz Shepherd, Mr. Shepherd, Ellis Shepherd, Maggie Pierce, Laura Grey-Thompson, Kathleen Shepherd, Thatcher Grey, Derek Shepherd, Susan Grey, Derek Bailey Shepherd, Winston Ndugu, Zola Grey Shepherd, Ellis Grey, Carolyn Shepherd, Amelia Shepherd

romances
: Derek Shepherd, Finn Dandridge, William Thorpe, Nathan Riggs, Andrew DeLuca, Cormac Hayes

doctors
: None

Now we can create a network based on the characters' relationships!

(We've coloured the nodes based on whether the character is alive or deceased (and edges based on relationship).)

Try our interactive plot to see who is connected! You can zoom in and out for closer looks.

<div align="center">
    <iframe src="inter.html" sandbox="allow-same-origin allow-scripts" width=700px height=700px></iframe>
</div>

We can see that some of the...

---

## Distributions

In ultrices, est at lobortis pretium, magna quam mollis neque, id viverra odio est sit amet lorem. Mauris efficitur nunc vel lectus porttitor, sit amet sodales quam eleifend. Duis et felis ut mauris dignissim efficitur. Aliquam non sem eros. Integer elit ante, bibendum id hendrerit vitae, vestibulum eget risus. Nunc efficitur nisl in iaculis vestibulum.

The in-degree distribution can be seen below...

![static network](images/in_degree.png)

SOMETHING CLEVER ABOUT THE DISTRIBUTION

The out-degree distribution can be seen below...

![static network](images/out_degree.png)

SOMETHING CLEVER ABOUT THE DISTRIBUTION

The degree distributions show that a lot of characters have very few connections, which is often the case for patients. The characters with high degrees are mainly the doctors who are also the main characters of the series. Let's have a closer look at these characters by exploring some statistics! Yay statistics!

---

## Statistics

First we'll look at which characters have the most connections.

Har gjort det på in-degree her - skal vi bare tage degree? eller både in/out?

<table style="color:white">
    <thead>
        <tr>
            <th style="color:white">#</th>
            <th>&nbsp;</th>
            <th style="color:white">Character</th>
            <th style="color:white">Connections</th>
            <th>&nbsp;</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td style="background-color:rgba(0, 0, 0, 0);"> 1</td>
            <td style="background-color:rgba(0, 0, 0, 0);">
                <img src="images/mer.jpg" class="img_c" alt="Meredith" height="100">
            </td>
            <td style="background-color:rgba(0, 0, 0, 0);">Meredith Grey</td>
            <td style="background-color:rgba(0, 0, 0, 0);">356</td>
        </tr>
        <tr>
            <td style="background-color:rgba(0, 0, 0, 0);"> 2 </td>
            <td style="background-color:rgba(0, 0, 0, 0);">
                <img src="images/karev.jpg" class="img_c" alt="Karev" height="100">
            </td>
            <td style="background-color:rgba(0, 0, 0, 0);">Alex Karev</td>
            <td style="background-color:rgba(0, 0, 0, 0);">300</td>
        </tr>
        <tr>
            <td style="background-color:rgba(0, 0, 0, 0);"> 3 </td>
            <td style="background-color:rgba(0, 0, 0, 0);">
                <img src="images/derek.jpg" class="img_c" alt="Derek" height="100">
            </td>
            <td style="background-color:rgba(0, 0, 0, 0);">Derek Shepherd</td>
            <td style="background-color:rgba(0, 0, 0, 0);">299</td>
        </tr>
         <tr>
            <td style="background-color:rgba(0, 0, 0, 0);"> 4 </td>
            <td style="background-color:rgba(0, 0, 0, 0);">
                <img src="images/bailey.jpg" class="img_c" alt="Miranda" height="100">
            </td>
            <td style="background-color:rgba(0, 0, 0, 0);">Miranda Bailey</td>
            <td style="background-color:rgba(0, 0, 0, 0);">289</td>
        </tr>
         <tr>
            <td style="background-color:rgba(0, 0, 0, 0);"> 5 </td>
            <td style="background-color:rgba(0, 0, 0, 0);">
                <img src="images/yang.jpg" class="img_c" alt="Yang" height="100">
            </td>
            <td style="background-color:rgba(0, 0, 0, 0);">Cristina Yang</td>
            <td style="background-color:rgba(0, 0, 0, 0);">252</td>
        </tr>
         <tr>
            <td style="background-color:rgba(0, 0, 0, 0);"> 6 </td>
            <td style="background-color:rgba(0, 0, 0, 0);">
                <img src="images/richard.jpg" class="img_c" alt="Richard" height="100">
            </td>
            <td style="background-color:rgba(0, 0, 0, 0);">Richard Webber</td>
            <td style="background-color:rgba(0, 0, 0, 0);">236</td>
        </tr>
         <tr>
            <td style="background-color:rgba(0, 0, 0, 0);"> 7 </td>
            <td style="background-color:rgba(0, 0, 0, 0);">
                <img src="images/hunt.jpg" class="img_c" alt="Hunt" height="100">
            </td>
            <td style="background-color:rgba(0, 0, 0, 0);">Owen Hunt</td>
            <td style="background-color:rgba(0, 0, 0, 0);">228</td>
        </tr>
</table>

Not surprising that the characters with most connections are the doctors and the characters that have been in the series for a long time. However, the creators of Grey's Anatomy are not shy of 'killing' the doctors whos lives we follow (RIP Derek), so let's have a look at their 'lifetime'.

The **125** attendings, residents and interns have an average 'lifetime' of **53** episodes or approximately **2** seasons. That doesn't sound like a lot! As you can see on the plot below the interquartile range is quite low but there is also quite a large variation.

Hover over the plot to see who has been in most episodes!

<script src="https://cdn.plot.ly/plotly-latest.min.js"></script>
<div align="center">                            <div id="11b60343-3b0a-4968-adc9-6325e5cd5b57" class="plotly-graph-div" style="height:100%; width:600px;"></div>            <script type="text/javascript">                                    window.PLOTLYENV=window.PLOTLYENV || {};                                    if (document.getElementById("11b60343-3b0a-4968-adc9-6325e5cd5b57")) {                    Plotly.newPlot(                        "11b60343-3b0a-4968-adc9-6325e5cd5b57",                        [{"alignmentgroup":"True","boxpoints":"all","hovertemplate":"<b>%{hovertext}</b><br><br>Count=%{y}<extra></extra>","hovertext":["Reed_Adamson","Teddy_Altman","Jackson_Avery","Miranda_Bailey","Kai_Bartley","Sam_Bello","Jeremy_Bennett","Naomi_Bennett","Sam_Bennett","Penelope_Blake","Lauren_Boswell","Ethan_Boyd","Hannah_Brody","Heather_Brooks","Preston_Burke","Leo_Byrider","Alana_Cahill","Julia_Canner","Walter_Carr","Paul_Castello","Marie_Cerone","James_Chee","Elizabeth_Chen","Claire_(Intern)","Cynthia_Cole","Isaac_Cross","Finn_Dandridge","Surgeon_Dave","Andrew_DeLuca","Carina_DeLuca","Vincenzo_DeLuca","Virginia_Dixon","Stephanie_Edwards","Lucy_Fields","Kevin_Fisher","Catherine_Fox","Cooper_Freedman","Lexie_Grey","Meredith_Grey","Graciella_Guzman","Erica_Hahn","Pierce_Halley","David_Hamilton","Sadie_Harris","Cormac_Hayes","Taryn_Helm","Nicole_Herman","Sydney_Heron","Megan_Hunt","Owen_Hunt","Intern_James","Alex_Karev","Jo_Wilson","April_Kepner","Reza_Khan","Nico_Kim","Dr._Knox","Tom_Koracick","Laura","Oliver_Lebackes","Michelle_Lin","Atticus_Lincoln","Intern_Lisa","Logan","Lucy","Graham_Maddox","Dani_Mandvi","Emma_Marling","Colin_Marlow","Nick_Marsh","Dr._McQueen","Dr._Milton","Eliza_Minnick","Addison_Forbes_Montgomery","Archer_Montgomery","Steve_Mostow","Leah_Murphy","Jason_Myers","Winston_Ndugu","Jim_Nelson","Megan_Nowland","George_OMalley","Alma_Ortiz","Sara_Ortiz","Casey_Parker","Darren_Parker","Daisy_Pepman","Charles_Percy","Zander_Perez","Andrew_Perkins","Morgan_Peterson","Maggie_Pierce","Dahlia_Qadri","Nathan_Riggs","Lauren_Riley","Arizona_Robbins","Shane_Ross","Vikram_Roy","Jeff_Russell","Connie_Ryan","Levi_Schmitt","Raj_Sen","Norman_Shales","Audrey_Shaw","Amelia_Shepherd","Derek_Shepherd","Blake_Simms","Mark_Sloan","Ryan_Spalding","Mitchell_Spencer","Paul_Stadler","Robert_Stark","Izzie_Stevens","Rebecca_Swender","Cecil_Taylor","Craig_Thomas","William_Thorpe","Callie_Torres","Mabel_Tseng","Violet_Turner","Michelle_Velez","Richard_Webber","Pete_Wilder","Katharine_Wyatt","Cristina_Yang"],"legendgroup":"","marker":{"color":"#636efa"},"name":"","notched":false,"offsetgroup":"","orientation":"v","showlegend":false,"x0":" ","xaxis":"x","y":[10,119,263,389,3,12,10,68,114,20,3,2,19,22,62,19,5,5,2,2,3,8,3,16,2,18,9,2,112,63,3,3,112,8,2,73,113,115,384,24,25,21,3,8,26,63,13,8,12,294,2,343,191,193,6,40,41,54,19,2,2,53,2,3,8,3,19,7,3,5,2,3,11,170,8,37,45,7,19,3,26,105,3,10,29,4,2,13,12,7,5,156,27,45,2,213,46,16,4,2,81,8,3,2,222,246,9,139,14,6,4,7,110,3,4,5,4,239,13,108,2,379,100,9,221],"y0":" ","yaxis":"y","type":"box"}],                        {"boxmode":"group","font":{"color":"white"},"legend":{"tracegroupgap":0},"margin":{"t":60},"paper_bgcolor":"rgba(0, 0, 0, 0)","template":{"data":{"barpolar":[{"marker":{"line":{"color":"#E5ECF6","width":0.5},"pattern":{"fillmode":"overlay","size":10,"solidity":0.2}},"type":"barpolar"}],"bar":[{"error_x":{"color":"#2a3f5f"},"error_y":{"color":"#2a3f5f"},"marker":{"line":{"color":"#E5ECF6","width":0.5},"pattern":{"fillmode":"overlay","size":10,"solidity":0.2}},"type":"bar"}],"carpet":[{"aaxis":{"endlinecolor":"#2a3f5f","gridcolor":"white","linecolor":"white","minorgridcolor":"white","startlinecolor":"#2a3f5f"},"baxis":{"endlinecolor":"#2a3f5f","gridcolor":"white","linecolor":"white","minorgridcolor":"white","startlinecolor":"#2a3f5f"},"type":"carpet"}],"choropleth":[{"colorbar":{"outlinewidth":0,"ticks":""},"type":"choropleth"}],"contourcarpet":[{"colorbar":{"outlinewidth":0,"ticks":""},"type":"contourcarpet"}],"contour":[{"colorbar":{"outlinewidth":0,"ticks":""},"colorscale":[[0.0,"#0d0887"],[0.1111111111111111,"#46039f"],[0.2222222222222222,"#7201a8"],[0.3333333333333333,"#9c179e"],[0.4444444444444444,"#bd3786"],[0.5555555555555556,"#d8576b"],[0.6666666666666666,"#ed7953"],[0.7777777777777778,"#fb9f3a"],[0.8888888888888888,"#fdca26"],[1.0,"#f0f921"]],"type":"contour"}],"heatmapgl":[{"colorbar":{"outlinewidth":0,"ticks":""},"colorscale":[[0.0,"#0d0887"],[0.1111111111111111,"#46039f"],[0.2222222222222222,"#7201a8"],[0.3333333333333333,"#9c179e"],[0.4444444444444444,"#bd3786"],[0.5555555555555556,"#d8576b"],[0.6666666666666666,"#ed7953"],[0.7777777777777778,"#fb9f3a"],[0.8888888888888888,"#fdca26"],[1.0,"#f0f921"]],"type":"heatmapgl"}],"heatmap":[{"colorbar":{"outlinewidth":0,"ticks":""},"colorscale":[[0.0,"#0d0887"],[0.1111111111111111,"#46039f"],[0.2222222222222222,"#7201a8"],[0.3333333333333333,"#9c179e"],[0.4444444444444444,"#bd3786"],[0.5555555555555556,"#d8576b"],[0.6666666666666666,"#ed7953"],[0.7777777777777778,"#fb9f3a"],[0.8888888888888888,"#fdca26"],[1.0,"#f0f921"]],"type":"heatmap"}],"histogram2dcontour":[{"colorbar":{"outlinewidth":0,"ticks":""},"colorscale":[[0.0,"#0d0887"],[0.1111111111111111,"#46039f"],[0.2222222222222222,"#7201a8"],[0.3333333333333333,"#9c179e"],[0.4444444444444444,"#bd3786"],[0.5555555555555556,"#d8576b"],[0.6666666666666666,"#ed7953"],[0.7777777777777778,"#fb9f3a"],[0.8888888888888888,"#fdca26"],[1.0,"#f0f921"]],"type":"histogram2dcontour"}],"histogram2d":[{"colorbar":{"outlinewidth":0,"ticks":""},"colorscale":[[0.0,"#0d0887"],[0.1111111111111111,"#46039f"],[0.2222222222222222,"#7201a8"],[0.3333333333333333,"#9c179e"],[0.4444444444444444,"#bd3786"],[0.5555555555555556,"#d8576b"],[0.6666666666666666,"#ed7953"],[0.7777777777777778,"#fb9f3a"],[0.8888888888888888,"#fdca26"],[1.0,"#f0f921"]],"type":"histogram2d"}],"histogram":[{"marker":{"pattern":{"fillmode":"overlay","size":10,"solidity":0.2}},"type":"histogram"}],"mesh3d":[{"colorbar":{"outlinewidth":0,"ticks":""},"type":"mesh3d"}],"parcoords":[{"line":{"colorbar":{"outlinewidth":0,"ticks":""}},"type":"parcoords"}],"pie":[{"automargin":true,"type":"pie"}],"scatter3d":[{"line":{"colorbar":{"outlinewidth":0,"ticks":""}},"marker":{"colorbar":{"outlinewidth":0,"ticks":""}},"type":"scatter3d"}],"scattercarpet":[{"marker":{"colorbar":{"outlinewidth":0,"ticks":""}},"type":"scattercarpet"}],"scattergeo":[{"marker":{"colorbar":{"outlinewidth":0,"ticks":""}},"type":"scattergeo"}],"scattergl":[{"marker":{"colorbar":{"outlinewidth":0,"ticks":""}},"type":"scattergl"}],"scattermapbox":[{"marker":{"colorbar":{"outlinewidth":0,"ticks":""}},"type":"scattermapbox"}],"scatterpolargl":[{"marker":{"colorbar":{"outlinewidth":0,"ticks":""}},"type":"scatterpolargl"}],"scatterpolar":[{"marker":{"colorbar":{"outlinewidth":0,"ticks":""}},"type":"scatterpolar"}],"scatter":[{"marker":{"colorbar":{"outlinewidth":0,"ticks":""}},"type":"scatter"}],"scatterternary":[{"marker":{"colorbar":{"outlinewidth":0,"ticks":""}},"type":"scatterternary"}],"surface":[{"colorbar":{"outlinewidth":0,"ticks":""},"colorscale":[[0.0,"#0d0887"],[0.1111111111111111,"#46039f"],[0.2222222222222222,"#7201a8"],[0.3333333333333333,"#9c179e"],[0.4444444444444444,"#bd3786"],[0.5555555555555556,"#d8576b"],[0.6666666666666666,"#ed7953"],[0.7777777777777778,"#fb9f3a"],[0.8888888888888888,"#fdca26"],[1.0,"#f0f921"]],"type":"surface"}],"table":[{"cells":{"fill":{"color":"#EBF0F8"},"line":{"color":"white"}},"header":{"fill":{"color":"#C8D4E3"},"line":{"color":"white"}},"type":"table"}]},"layout":{"annotationdefaults":{"arrowcolor":"#2a3f5f","arrowhead":0,"arrowwidth":1},"autotypenumbers":"strict","coloraxis":{"colorbar":{"outlinewidth":0,"ticks":""}},"colorscale":{"diverging":[[0,"#8e0152"],[0.1,"#c51b7d"],[0.2,"#de77ae"],[0.3,"#f1b6da"],[0.4,"#fde0ef"],[0.5,"#f7f7f7"],[0.6,"#e6f5d0"],[0.7,"#b8e186"],[0.8,"#7fbc41"],[0.9,"#4d9221"],[1,"#276419"]],"sequential":[[0.0,"#0d0887"],[0.1111111111111111,"#46039f"],[0.2222222222222222,"#7201a8"],[0.3333333333333333,"#9c179e"],[0.4444444444444444,"#bd3786"],[0.5555555555555556,"#d8576b"],[0.6666666666666666,"#ed7953"],[0.7777777777777778,"#fb9f3a"],[0.8888888888888888,"#fdca26"],[1.0,"#f0f921"]],"sequentialminus":[[0.0,"#0d0887"],[0.1111111111111111,"#46039f"],[0.2222222222222222,"#7201a8"],[0.3333333333333333,"#9c179e"],[0.4444444444444444,"#bd3786"],[0.5555555555555556,"#d8576b"],[0.6666666666666666,"#ed7953"],[0.7777777777777778,"#fb9f3a"],[0.8888888888888888,"#fdca26"],[1.0,"#f0f921"]]},"colorway":["#636efa","#EF553B","#00cc96","#ab63fa","#FFA15A","#19d3f3","#FF6692","#B6E880","#FF97FF","#FECB52"],"font":{"color":"#2a3f5f"},"geo":{"bgcolor":"white","lakecolor":"white","landcolor":"#E5ECF6","showlakes":true,"showland":true,"subunitcolor":"white"},"hoverlabel":{"align":"left"},"hovermode":"closest","mapbox":{"style":"light"},"paper_bgcolor":"white","plot_bgcolor":"#E5ECF6","polar":{"angularaxis":{"gridcolor":"white","linecolor":"white","ticks":""},"bgcolor":"#E5ECF6","radialaxis":{"gridcolor":"white","linecolor":"white","ticks":""}},"scene":{"xaxis":{"backgroundcolor":"#E5ECF6","gridcolor":"white","gridwidth":2,"linecolor":"white","showbackground":true,"ticks":"","zerolinecolor":"white"},"yaxis":{"backgroundcolor":"#E5ECF6","gridcolor":"white","gridwidth":2,"linecolor":"white","showbackground":true,"ticks":"","zerolinecolor":"white"},"zaxis":{"backgroundcolor":"#E5ECF6","gridcolor":"white","gridwidth":2,"linecolor":"white","showbackground":true,"ticks":"","zerolinecolor":"white"}},"shapedefaults":{"line":{"color":"#2a3f5f"}},"ternary":{"aaxis":{"gridcolor":"white","linecolor":"white","ticks":""},"baxis":{"gridcolor":"white","linecolor":"white","ticks":""},"bgcolor":"#E5ECF6","caxis":{"gridcolor":"white","linecolor":"white","ticks":""}},"title":{"x":0.05},"xaxis":{"automargin":true,"gridcolor":"white","linecolor":"white","ticks":"","title":{"standoff":15},"zerolinecolor":"white","zerolinewidth":2},"yaxis":{"automargin":true,"gridcolor":"white","linecolor":"white","ticks":"","title":{"standoff":15},"zerolinecolor":"white","zerolinewidth":2}}},"width":600,"xaxis":{"anchor":"y","domain":[0.0,1.0]},"yaxis":{"anchor":"x","color":"white","domain":[0.0,1.0],"title":{"text":"Count"}}},                        {"responsive": true}                    )                };                            </script>        </div>

Wauw, Miranda Bailey has been in 389 episodes! This means she is the most appearing character in the Grey's Anatomy franchise.

PLOTS OM VIEWS AF EPISODER/SÆSONER?

OVERGANG TIL ROMANCES

PLOT / TABLE

---

So now we have seen that the OG characters are the ones with most connections and that their 'lifetime' in the series varies quite a lot. For further analysis we will take a deeper look at some of these characters development over time...


