# Quick Start Guide

```danger
This page is under construction
```

## 1. Access Token & OAuth 2.0 Authentication
There are two main ways to access your Figma accounts, Access Token and OAuth ()

```tip
OAuth is recommended as it is more secure.
```

See this [link](https://www.figma.com/developers/api#access-tokens) to learn how to get Access tokens.

See this [link](https://www.figma.com/developers/api#oauth2) to learn how to get Access tokens.

## 3. Project File ID
The project ID of a Figma file is part of the share URL link of a project.

For Example:
If the link is

`https://www.figma.com/file/YpBnZ4aEB2YgGpiOQfxQCU/ExampleFile`

The project ID would be the following:

`YpBnZ4aEB2YgGpiOQfxQCU`

## 4. Selecting Screens
Simply select the pages that you would like to convert into React Native project.

Once selected, click **Convert to Code**. This will start the conversion process and will download as a `.zip` file once completed.

## 5. Running Project
The project is converted into React Native project. Therefore, it will require Node.js

### 5.1 Node.js & Expo
Requires Node.js LTS 12 or later - [download here](https://nodejs.org/en/).

Requires expo-cli - Assuming that you have Node 12 LTS or greater installed, you can use npm to install the Expo CLI command line utility:

```
npm install -g expo-cli
```

### 5.2 Initialising Project
```bash
expo init ProjectName
```

### 5.3 Copying Converted Files
The generated code based on the Figma project will need to be unzipped. 

The files will need to be copied to the newly initiated project within the **same** corresponding directories.

### 5.4 Install dependencies
```
yarn install
```
or
```
npm install
```

### 5.5 Run the App
```
yarn start
```
or
```
npm start
```

This command will start a development server on your machine. 

Install the [Expo](https://expo.io/) client app on your iOS or Android phone and connect to the same wireless network as your computer. 
On Android, use the Expo app to scan the QR code from your terminal to open your project. 
On iOS, use the built-in QR code scanner of the Camera app. 

Alternatively, you can set up an emulator - [more information here](https://reactnative.dev/docs/environment-setup)

