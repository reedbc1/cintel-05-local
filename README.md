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

### Export to docs folder
```shell
.venv\Scripts\Activate
shiny static-assets remove
shinylive export dashboard docs
py -m http.server --directory docs --bind localhost 8008
```
Open a browser to http://[::1]:8008/ and test the Pages app.

### Push Changes back to GitHub

Open a terminal (VS Code menu "Terminal" / "New Terminal") in the root project folder and run these commands.

```shell
git add .
git commit -m "Useful commit message"
git push -u origin main
```

### Enable GitHub Pages (One-Time)

Go to your GitHub repository settings. 
Scroll down to the Pages tab.
Enable GitHub Pages from the **main** branch and from the **docs** folder and click Save.
Wait to see what you new URL is for the hosted app.

When it's ready, go to the About section of your GitHub repo and set the URL to your GitHub Pages site.
