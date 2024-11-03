**Wed Oct 23**<br>
**MPAD2003A Introductory Data Storytelling**<br>
**Noor Choudhry**<br>
**Presented to Jean-Sébastien Marier**<br>

# Midterm Project: Exploratory Data Analysis (EDA)

Use one hashtag symbol (`#`) to create a level 1 heading like this one.

## Foreword

For this assignment, you must extract data from a dataset provided by the instructor. You must then clean and analyze the data, create exploratory charts/visualizations, and find a potential story idea. Your assignment must clearly detail your process. You are expected to write about 1500-2000 words, and to include several screen captures showing the different steps you went through. Your assignment must be written with the Markdown format and submitted on GitHub Classroom.

I have been assigning different versions of this project to my digital journalism and data storytelling students for a few years now. Its structure was inspired by the main sections/chapters of [*The Data Journalism Handbook*](https://datajournalism.com/read/handbook/one/). This version was further inspired by the [Key Capabilities in Data Science](https://extendedlearning.ubc.ca/programs/key-capabilities-data-science) program offered by the University of British Columbia (UBC).

**Here are some useful resources for this assignment:**

* [GitHub's *Basic writing and formatting syntax* page](https://docs.github.com/en/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax)
* [The template repository for this assignment in case you delete something by mistake](https://github.com/jsmarier/jou4100_jou4500_mpad2003_project2_template)

Did you notice how to create a hyperlink? In Markdown, we put the clickable text between square brackets and the actual URL between parentheses.

And to create an unordered list, we simply put a star (`*`) before each item.

## 1. Introduction

The purpose of this analysis is to explore a dataset from the City of Ottawa that documents a range of service requests submitted by residents during August 2024. The dataset encompasses various fields, including request type, description, status, opening and closing dates, address, and ward. This collection covers the city's public service responses across various regions, offering insights into service delivery and community needs.

I will **gather data** from the service request records of Ottawa and **investigate** it using a *VIMO analysis*, followed by *data cleaning* and a thorough *Exploratory Data Analysis* (EDA) to uncover trends and insights. Finally, I will use these insights to create visuals and build a **brief narrative** about service patterns across the city.

For the original dataset, [click here](https://open.ottawa.ca/documents/65fe42e2502d442b8a774fd3d954cac5/about). If you're interested in downloading the CSV file from Professor Jean-Sébastien Marier's GitHub page, you can [click here](https://raw.githubusercontent.com/jsmarier/course-datasets/refs/heads/main/ottawa-311-service-requests-august-2024.csv).

**Or copy and paste these links into your browser:**

Original dataset: https://open.ottawa.ca/documents/65fe42e2502d442b8a774fd3d954cac5/about 

CSV file:
https://raw.githubusercontent.com/jsmarier/course-

## 2. Getting Data

To import data into Google Sheets, download the CSV file using Professor Jean-Sébastien Marier's GitHub link to the CSV file ([click here](https://raw.githubusercontent.com/jsmarier/course-datasets/refs/heads/main/ottawa-311-service-requests-august-2024.csv)). I used the drag-and-drop feature on my MacBook to upload the CSV file onto Google Sheets. Alternatively, you can go through the following steps: select **File > Import > Upload > Select a file from your device**. In the import settings, select **Replace current sheet** for "Import location" and use a **comma** as the "Separator type" to get a proper column display. The dataset consists of 10 columns and approximately 29,000 rows (28,539 to be exact).

![](importfile-example.png)<br>
*Figure 1: The "Import file" prompt on Google Sheets.*

[Click here for my public link to the dataset on Google Sheets.](https://docs.google.com/spreadsheets/d/18Z9AKnIkgHHDtc3c6YVl4Flks-yFMDA5r0NuCJRX324/edit?usp=sharing)

Or copy & paste this link into your browser: https://docs.google.com/spreadsheets/d/18Z9AKnIkgHHDtc3c6YVl4Flks-yFMDA5r0NuCJRX324/edit?usp=sharing


![](googlesheets-screencapture.png)<br>
*Figure 2: Screen capture of my dataset in Google Sheets.*

### Observations of Key Columns

- **Status** (column B): A nominal (categorical) variable that shows the status of each request (options include: Active, Resolved, and Cancelled).
- **Opened Date and Closed Date** (columns E & F): These two are fields that can help analyze the duration of each request.
- **Ward** (column J): A discrete numerical variable that helps with th geographic analysis of requests across the city.

### General Observations

Some columns, such as **Address**, **Latitude**, and **Longitude**, have missing values, which could affect location-based analyses. The data appears clean in terms of categorical organization, but with so many rows, readability can be challenging. The dataset is well-organized by columns, but given the volume of entries, it will be difficult to analyze on its own.

### Hypothesis/Question

A question that comes to mind for this data involves exploring a possible correlation between **ward** and **service efficiency**. Specifically, I am interested in analyzing the relationship between ward location and response times for specific service requests, like road maintenance or health inspections, based on the **status**, **quantity**, and **type** of requests.


<br>
<br><br>
<br><br>
<br>
just want to keep this informoaton, but separated incase i need it
<br>
<br>

Use two hashtag symbols (`##`) to create a level 2 heading like this one.

To include a screen capture, use the sample code below. Your images should be saved in the same folder as your `.md` file.


![](importfile-example.png)<br>
*Figure 1: The "Import file" prompt on Google Sheets.*

**Here are examples of functions and lines of code put in grey boxes:**

1. If you name a function, put it between "angled" quotation marks like this: `IMPORTHTML`.
1. If you want to include the entire line of code, do the same thing, albeit with your entire code: `=IMPORTHTML("https://en.wikipedia.org/wiki/China"; "table", 5)`.
1. Alternatively, you can put your code in an independent box using the template below:

``` r
=IMPORTHTML("https://en.wikipedia.org/wiki/China"; "table", 5)
```
This also shows how to create an ordered list. Simply put `1.` before each item.

## 3. Understanding Data

### 3.1. VIMO Analysis

Use three hashtag symbols (`###`) to create a level 3 heading like this one. Please follow this template when it comes to level 1 and level 2 headings. However, you can use level 3 headings as you see fit.

Insert text here.

Support your claims by citing relevant sources. Please follow [APA guidelines for in-text citations](https://apastyle.apa.org/style-grammar-guidelines/citations).

**For example:**

As Cairo (2016) argues, a data visualization should be truthful...

### 3.2. Cleaning Data

Insert text here.

### 3.3. Exploratory Data Analysis (EDA)

Insert text here.

**This section should include a screen capture of your pivot table, like so:**

![](pivot-table-screen-capture.png)<br>
*Figure 2: This pivot table shows...*

**This section should also include a screen capture of your exploratory chart, like so:**

![](chart-screen-capture.png)<br>
*Figure 3: This exploratory chart shows...*

## 4. Potential Story

Insert text here.

## 5. Conclusion

Insert text here.

## 6. References

Include a list of your references here. Please follow [APA guidelines for references](https://apastyle.apa.org/style-grammar-guidelines/references). Hanging paragraphs aren't required though.

**Here's an example:**

Bounegru, L., & Gray, J. (Eds.). (2021). *The Data Journalism Handbook 2: Towards A Critical Data Practice*. Amsterdam University Press. [https://ocul-crl.primo.exlibrisgroup.com/permalink/01OCUL_CRL/hgdufh/alma991022890087305153](https://ocul-crl.primo.exlibrisgroup.com/permalink/01OCUL_CRL/hgdufh/alma991022890087305153)
