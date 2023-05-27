# IdahoAirstrips_ForeflightPack
Creates a Foreflight pack from the Idaho airstrips listed on idahoaviation.com


## Data Gathering
Data was gathered from idahoaviation.org
List of airports and relevant links was copied from the page source - this was done to minimize effort.

Using the list of airports each airport's page was scraped for information such as management, runway details, description etc.

# Templates and rendering
I used the foreflight pack from Utah Backcountry Pilots as a template.
The files were templatized to use jinja2 as a template rendering engine.
The data gathered from the first step was used to render the templates.

# Pack generation
The content pack allows us to render custom content in foreflight.
More details can be found (here))[https://foreflight.com/products/foreflight-mobile/user-content/content-packs/]

The bottom of the notebook contains some basic shell commands to create a folder, copy the generated file into the colder and then zip it up.

The zipped folder is what foreflight wants to receive the content pack.

# Runing the code 

Install the dependencies using 

`pip install -r requirements.txt`

start juputer using 

`jupyter notebook`

Run the notebook named `idaho_scraper.ipynb`
