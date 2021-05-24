# World-Bank-Data-Dashboard
This is a python Flask app data dashboard that pulls data from the World Bank API. The visualizations are made with the plotly library.

Code and files.
The code contains a python scrpt called `wrangle_data.py`:

`1`This script contains a cleandata function to clean world bank data for a visualizaiton dashboard. It keeps data range of dates in keep_columns variable
  and data for the top 10 economies, reorients the columns into a year, country and value then saves the results to a csv file.
  
`2`It also contains a returnfigures function that creates data visualisations from the world bank data
  
 # Getting Started

To get the app working locally:
1. Clone or download the repository locally
2. Within the world_bank_api_dashboard directory, create a virtual Python environment with the Terminal command `python3 -m venv flaskapp` where `flaskapp` is the name of your environment. You can choose any name.
3. Activate the virtual environment with the command `source flaskapp/bin/activate`
4. Then run the command `pip install -r requirements.txt`
5. Next, set the FLASK_APP variable to worldbank.py by running the following command `export FLASK_APP=worldbank.py`.
6. And finally, run the command `python -m flask run` to start the app
7. The terminal will output the local web address and port where the app is running. As an example, this might be `http://127.0.0.1:5000/`. Now, open a web browser and go to that web address.

# Prerequisites

You will need [Python3 installed](https://www.python.org/downloads/) on your local machine.

# Deployment

Flask apps can be deployed to a variety of platforms. Here is an example for deploying the web app with Heroku.

1. Install the Heroku [command line interface](https://devcenter.heroku.com/articles/getting-started-with-python#set-up)
2. Then, in the command line enter `heroku login` and enter your account name and password
3. Cd into the world_bank_api_dashboard repository folder
4. In the command line, enter `heroku create`
5. Then enter `git push heroku master`
6. And finally 'heroku open'

# Built With
* [Python](https://www.python.org/) - programming language
* [Flask](http://flask.pocoo.org/) - web development framework
* [Pandas](https://pandas.pydata.org/) - data manipulation and analysis
* [Plotly](https://plot.ly/python/) - data visualization library
