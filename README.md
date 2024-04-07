# README
## Instructions for setting up local workspace
### Cloning repo
- Open VSCode and clone repository.
- Copy the cintel-05-local github repo link and paste.
- Select folder you would like to save the repository to.  
### Creating virtual environment
- Open a terminal, making sure that the directory is the repo directory.
- Enter python -m venv .venv
### Activating environment
- Enter .venv\Scripts\activate
- **Do this every time you open this folder in a fresh workspace.**
### Installing dependencies
- Enter pip install -r requirements.txt  
- This only needs to be done once for the virtual environment.
## Running PyShiny Locally
- Open a terminal in the project directory
- Enter shiny run --reload --launch-browser dashboard/app.py
- Open a browser to http://127.0.0.1:8000/ and test the app.
