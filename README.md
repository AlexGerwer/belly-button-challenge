# Belly Button Biodiversity Dashboard

This interactive dashboard explores the Belly Button Biodiversity dataset, visualizing the bacterial cultures found in human navels.  Users can select different sample IDs to view the demographic information and the diversity of bacterial species present in that individual's belly button.

## Project Overview

This project uses D3.js and Plotly.js to create interactive charts and displays demographic information dynamically based on user selection. It fetches data from a JSON file (`samples.json`) and renders a bar chart, a bubble chart, and a metadata panel.  The project demonstrates efficient data handling, clear display, and robust error management.


## Dashboard Features

* **Interactive Dropdown:** Select a test subject ID from the dropdown menu to explore their belly button biodiversity data.
* **Demographic Info Panel:** Displays demographic information for the selected test subject, including ID, ethnicity, gender, age, location, belly button type, and washing frequency.
* **Bar Chart:** Shows the top 10 bacterial species (OTUs) found in the selected individual's belly button, ranked by abundance.  The chart uses formatted OTU labels for clarity.
* **Bubble Chart:**  A bubble chart visualizes the relative abundance of each OTU in the sample.  The size of each bubble represents the sample value, and the color represents the OTU ID, with an "Earth" colorscale applied.  The x-axis represents the OTU ID.

## Files and Folders
```text
belly-button-challenge/
├── Belly Button Biodiversity – Public Science Lab.pdf # a description of the data source used in generating this repo's results
├── index.html # Main HTML file for the dashboard
├── samples.json # Data file containing sample data
├── app_js_explanation.pdf # an explanation of the Javascript code in the app.js file
├── app_js_output.pdf # the output in a local Chrome browser and the output of the browser developer tools
├── README.md # This file
└── static/
    └── js/
        ├── app.js # JavaScript for charts and interaction, containing the dashboard logic
        └── samples.json # Data file (often a symbolic link to ../samples.json)
```

## Data Source

The data used in this project is sourced from the Belly Button Biodiversity dataset.  The `samples.json` file contains information about bacterial cultures found in the belly buttons of different individuals, along with their demographic data.

## Technologies Used

* **D3.js:**  Used for data manipulation and binding data to the DOM.
* **Plotly.js:** Used for creating interactive charts (bar chart and bubble chart).
* **HTML:**  Structure and layout of the dashboard.
* **CSS (Bootstrap):** Styling and layout.
* **JavaScript:**  Dashboard logic and interaction.

## Key Code Features

* **Error Handling:** Comprehensive `.catch()` blocks are used for robust error management throughout the code to handle potential issues during data fetching and processing.
* **Clarity and Readability:**  The code is formatted for easy readability and well-commented to explain the logic and purpose of different sections.
* **Efficiency:** Data is fetched only once during the initialization (`init()`) function for optimal performance, avoiding redundant data requests.

## Deployment

This project is designed to be deployed as a static website, ideally using GitHub Pages. 

The necessary steps have already been taken to configure the repository for deployment.  The site is configured to deploy from the `main` branch.

After pushing the `docs` folder containing `index.html`, `app.js`, `styles.css`, and `samples.json` to the `main` branch, GitHub Pages automatically builds and deploys the website. The deployment status can be monitored in the "Pages" section of the repository settings.

The website will be accessible at: `https://AlexGerwer.github.io/belly-button-challenge/`.

## How to Use

1. Clone the repository to your local machine.
2. Open `index.html` in a web browser.
3. Select a test subject ID from the dropdown menu to view their data. The charts and metadata panel will update dynamically.



## License

This project is licensed under the MIT License.
