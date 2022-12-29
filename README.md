# Home Geinie Application

This application is Home Genie smart application. This is hosted [here](https://home-genie-6fc05.web.app) for preview and the below instructions are tested for a stable development workflow.

## Getting Started
* [Download the installer](https://nodejs.org/) for Node LTS.
* Install the ionic CLI globally: `npm install -g ionic`
* Clone this repository: `git clone https://github.com/pavanpaik/home-genie.git`.
* Configure xCode with cocoapods : `sudo gem install -n /usr/local/bin cocoapods `

### Build/Development steps
* Angular application install -  `npm install --force`
* Browser based Build & Test - `ionic serve` 
* Application Build - `npm run build` (This will generate a /www sub folder with the html+javascript pwa application that can be deployed into any platform)
* Platform 
 * Add Platforms ios -  `npx cap add ios` (This will generate /ios sub folder which can then be deployed as an ios app) 
 * Add Platforms android -  `npx cap add android` (This will generate /android sub folder which can then be deployed as an ios app) 
 * Sync Platforms - `npx cap sync`
* Firebase Web Hosting
  * Login to firebase using cli - `firebase login`
  * Select the project to use - `firebase use home-genie-6fc05`
  * Deploy the project - `firebase deploy`

#### PLatform - IOS
* Deploy & Test - `npx cap run ios`
* Deploy & Test this project  uisng xcode - `npx cap open ios`

#### PLatform - Android
* Deploy & Test - `npx cap run android`
* Deploy & Test this project uisng AndroidStudio - `npx cap open android`

Follow Official Capsitor Development Workflow instructions [here](https://capacitorjs.com/docs/basics/workflow)
