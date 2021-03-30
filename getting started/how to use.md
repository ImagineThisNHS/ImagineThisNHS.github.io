# Quick Start Guide

## 1. Open the ImagineThis web app
Go to our deployed version [here](http://212.71.234.198/) or get it running locally.

To run everything locally, you need to clone both the 'ImagineThisServer' and 'imaginethisweb' repositories and follow their respective readmes to get them up and running.

## 2. Access Token & OAuth 2.0 Authentication
Once you get into our web interface, there are two main ways to access your Figma accounts: Access Token and OAuth. Select one of them and continue.

```tip
OAuth is recommended as it is more secure. (And very easy to use)
```
See this [link](https://www.figma.com/developers/api#access-tokens) to learn how to get Access tokens.
See this [link](https://www.figma.com/developers/api#oauth2) to learn more about OAuth.

## 3. Project File ID
Next you will need to provide a project ID of a Figma file that you wish to convert. The project ID of a Figma file is part of the share URL link of a project.

For Example:
If the link is

`https://www.figma.com/file/YpBnZ4aEB2YgGpiOQfxQCU/ExampleFile`

The project ID would be the following:

`YpBnZ4aEB2YgGpiOQfxQCU`

## 4. Selecting Screens
Simply select the pages that you would like to convert into React Native project by selecting/unselecting all with a button or clicking on them individually.

Once selected, click **Convert to Code**. This will start the conversion process and will download the generated source code in a `.zip` file once completed.

## 5. Sharing project
If you want to share the project with other users, you simply share the URL of the project page or share the project ID.

## 6. Run app through ImagineThis
Follow the instruction on ImagineThis website and scan the QR-code in order to run the app on your phone.

## 7. Run app locally
We generate a complete React Native project source code out of your Figma screens. To run it, please follow the steps below:

### 7.1 Prerequisites - Getting Node.js & Expo
Requires Node.js LTS 12 or later - [download here](https://nodejs.org/en/).

Requires expo-cli - Assuming that you have Node 12 LTS or greater installed, you can use npm to install the Expo CLI command line utility:

```
npm install -g expo-cli
```

### 7.2 Initialising a New Expo Project
```bash
expo init ProjectName
```
When prompted, select a blank template within terminal.

### 7.3 Copying Converted Files
The generated code based on the Figma project will need to be unzipped. 

The files will need to be copied to the newly initiated project within the **same** corresponding directories.

#### Please Note:
When copying files be sure to only replace existing files with the generated code downloaded. Do not delete any files that are created by default from the template file.

### 7.4 Install dependencies
Enter the directory of the project just created 

Then run:

```
npm install
```

### 7.5 Start the development server

```
npm start
```

This command will start a development server on your machine. 
### 7.6 Run your app on your device

#### 7.6.1 Run on mobile device
Install the [Expo](https://expo.io/) client app on your iOS or Android phone and connect to the same wireless network as your computer. 
On Android, use the ```Scan QR Code``` function in Expo app to scan the QR code from your terminal to open your project. 
On iOS, use the device's built-in camera app to scan the QR code.

Alternatively, you can set up an emulator - [more information here](https://reactnative.dev/docs/environment-setup)

#### 7.6.2 Run in web browser
You can also run the generated prototype on your web browser. Select the ```Run in web brower``` mode in the development page. The generated prototype will be automatically run in your web browser.


## Extra - Working with source code
### Beautifying the Code
By default, the code will not be indented correctly because it would be extremely challenging to keep track of the correct indents throughout all the layers of our conversion process.

However, it is extremely easy to format and beautify the file to your preferred indentation setup by using the built in features of modern code editors (or their plugins).

```tip
We strongly recommend using Visual Studio Code to handle your react-native project as it has great javascript-specific built-in features. One of them is built in javascript code formatter (Right click + Format Document, or simply 'Shift+Alt+F')
```


