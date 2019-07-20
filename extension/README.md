# Chrome Geolocation Spoof Extension
Chrome extension for spoofing geolocation.  
Mainly used for development of GPS applications.  
  
This project is based on Angular scaffold project (template) for google chrome extensions, see [Github.](https://github.com/larscom/angular-chrome-extension)

## How to use/develop
- run `npm install`
- run `npm run watch`
- goto: `chrome://extensions` in the browser and enable 'developer mode'
- press `Load unpacked` and target the folder `angular/dist`

The project is automatically being watched, any changes to the files will recompile the project.
**NOTE**: changes to the contentPage/backgroundPage requires you to reload the extension in `chrome://extensions`

## Build/package for production
- run `npm run build:production`
- upload `extension-build.zip` to the chrome webstore.
- (optional) you can also manually zip your extension, the production build will output to folder `angular/dist`

This will run a production build and will automatically zip it as a extension package in the root folder `./` named: `extension-build.zip`
**NOTE**: Do not forget to update the version number inside `manifest.json`

## Angular folder
This folder contains the angular source code.

## Chrome folder
This folder contains the contentPage/backgroundPage script for the google chrome extension
