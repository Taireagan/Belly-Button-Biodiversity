<div align="center">
    <h1>Belly Button Biodiversity</h1>
</div>


<div align="center">
    <h4>By: Tai Reagan</h4>
</div>

![microbes](https://github.com/Taireagan/Belly-Button-Biodiversity/blob/main/Images/microbes-sem.jpg)

<div  align="right";">
  Image Source: The Public Science Lab
</div>

---

## Background
This project involves building an interactive dashboard to explore the [Belly Button Biodiversity dataset](https://robdunnlab.com/projects/belly-button-biodiversity/) dataset, which catalogs the microbes that colonize human navels. The dataset provides insights into microbial diversity by identifying operational taxonomic units (OTUs) found in different individuals. Interestingly, the study reveals that while a small number of microbial species are present in over 70% of people, most species are relatively rare.

The interactive dashboard allows users to visualize and analyze this data, making it easier to explore which microbial species are common or rare across individuals. Through dynamic charts and informative panels, users can dive into the microbial makeup of belly buttons and better understand human microbiome diversity.

## Tools 
These are the tools, techniques, and resources used in this project.

- Plotly is used in combination with D3 and Javascript to generate the plots

- HTML is used for the framework of the page

- Github Pages is used to host the data and final application

- The data is stored in JSON format and imported in

## Step 1: Create a Horizontal Bar Chart
In this step, the D3 library was used to read the samples.json file from the URL **https://static.bc-edx.com/data/dl-1-2/m14/lms/starter/samples.json**. This JSON file contains microbiome data for different individuals. Then created a horizontal bar chart that displays the top 10 OTUs (Operational Taxonomic Units) found for a selected individual. The chart includes the following components:

- **sample_values** are used as the values for the bars.
- **otu_ids** are used as the labels for the bars.
- **otu_labels** are displayed as hover text for additional context when hovering over the bars.
- 
A dropdown menu allows users to select an individual, and the chart updates dynamically to reflect the top 10 OTUs for that selection.

  ![bar chart](https://github.com/Taireagan/Belly-Button-Biodiversity/blob/main/Images/bar%20chart.png)

## Step 2: Create a Bubble Chart
In this step, bubble chart was created to visualize each sample's microbiome data. The chart is designed to show the relationship between different OTUs (Operational Taxonomic Units) and their abundance in a given sample.
- **otu_ids** are used for the x-axis values.
- **sample_values** are used for the y-axis values, representing the abundance of each OTU.
- **sample_values** are also used to determine the size of each marker (bubble).
- **otu_ids** are used to color the markers, distinguishing different OTUs.
- **otu_labels** are displayed as hover text, providing additional information about each OTU.

This interactive bubble chart allows users to explore the distribution and abundance of OTUs across samples, with visual cues like color and size representing various dimensions of the data.

![bubble chart](https://github.com/Taireagan/Belly-Button-Biodiversity/blob/main/Images/bubble%20chart.png)

## Step 3: Display Sample Metadata
In this step, the demographic information of the selected individual by accessing their metadata from the JSON file was showcased in a display chart. By looping through each key-value pair in the individual's metadata JSON object. For each key-value pair, a text string was created so that it presents the demographic data (e.g., Age: 34). Then appended an HTML element containing this text to the #sample-metadata panel on the dashboard.

By presenting the individual's metadata, users can gain insights into the demographic factors associated with the microbiome samples. This information enhances the dashboard's interactivity and provides context for the microbiome data visualizations.  


<div align="center">
    <img src="https://github.com/Taireagan/Belly-Button-Biodiversity/blob/main/Images/demographics.png" alt="demographics" alt="crowdfunding_image"/>
</div>


## Final Step: Visualization
Finally updated all the plots when a new sample is selected and deployed app to a free static page hosting service (GitHub Pages).

![visualization](https://github.com/Taireagan/Belly-Button-Biodiversity/blob/main/Images/visualization.png)



### References:
Hulcr, J. et al. (2012) A Jungle in There: Bacteria in Belly Buttons are Highly Diverse, but Predictable. 

Retrieved from:

[RThe Public Science Lab](https://robdunnlab.com/projects/belly-button-biodiversity/results-and-data/)
