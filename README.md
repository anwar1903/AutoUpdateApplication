## Step 1:
        Install Electron, Electron Builder
         npm install --save-dev electron  (version: 7.1.2)
                npm add electron-builder --only=dev (version: 21.2.0).
                
## Step 2:
        1. write a Following code to [index.js]("https://github.com/anwar1903/AutoUpdateApplication/blob/dev/index.js") file 
        See in dev branch..
       
## Step 3:
        Create a Index.html File and import into the index.js file
        
## Step 4:
        Now go to Package.json file and add build property
        // see in dev branch package.json file
    
## Step 5:
        Go to GitHub and create a repository and get the token for that repository
        and add it to the package.json file.

## Step 6:
        Now we create electron-builder.yml file.  Add the appId, provider property inside it.
        And also create .gitignore file and write electron-builder.yml 
          this means that when the project is build electron-builder cannot be included in the build file.
         
## Step 7:
        Run the project.
          Code: npm run deploy
       
## Step 8:
        Check the Release Tab in the github...
