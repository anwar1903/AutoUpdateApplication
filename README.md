## Step 1:
- Install Electron, Electron Builder
        ``` npm install --save-dev electron  (version: 7.1.2) ```
        ``` npm add electron-builder --only=dev (version: 21.2.0) ```
                
## Step 2:
- write a Following code to `index.js` file 
       [Click to GO](https://github.com/anwar1903/AutoUpdateApplication/blob/dev/index.js#L1)
       
## Step 3:
- Create a Index.html File and import into the index.js file
        [index.html](https://github.com/anwar1903/AutoUpdateApplication/blob/dev/index.html)
        
## Step 4:
- Now go to `Package.json` file and add build property
        [file](https://github.com/anwar1903/AutoUpdateApplication/blob/dev/package.json)
    
## Step 5:
- Go to [GitHub](https://github.com) and create a [repository](https://github.com/new) and get the token for that repository
        and add it to the `package.json` file.

## Step 6:
- Now we create `electron-builder.yml` file.  Add the appId, provider property inside it.
        And also create `.gitignore` file and write `electron-builder.yml` 
          this means that when the project is build electron-builder cannot be included in the build file.
- Inside `electron-builder.yml`, we can declare,
   ``` appId: com.example.app
       publish: 
         provider: github
         token: YOUR GITHUB TOKEN  ```
         
## Step 7:
- Run the project.
              ``` npm run deploy ```
       
## Step 8:
        Check the Release Tab in the github...
