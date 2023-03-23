# Chrome Extension Boilerplate with Manifest 3
This is a basic boilerplate for creating a Chrome Extension with Manifest 3. It includes the necessary files and folder structure to get started quickly.

## Folder Structure
The folder structure is as follows:

```
my-extension/
├── extension/
│   ├── background.js
│   ├── content.js
│   ├── icons/
│   │   ├── icon16.png
│   │   ├── icon32.png
│   │   ├── icon48.png
│   │   └── icon128.png
│   ├── popup/
│   │   ├── popup.html
│   │   └── popup.js
│   └── manifest.json
├── src/
│   └── // source files for the extension
├── webpack.config.js
├── babel.config.js
├── package.json
└── node_modules/
    └── // dependencies installed by npm

```

## Getting Started
To use this boilerplate, follow these steps:

- Clone the repository or download the ZIP file.
- Edit manifest.json file to add the required information about the extension.
- Customize popup.html as per your needs.
- Add your own JavaScript code in src/index.js.
- Load the extension in Chrome by navigating to chrome://extensions, enabling "Developer mode" in the top right corner, and then clicking on "Load unpacked" and selecting the folder that contains the extension files.

### Manifest.json
The manifest.json file is the main configuration file for the extension. It contains information such as the extension's name, version, description, icons, permissions, and background scripts.

Make sure to update the fields in manifest.json with the appropriate values for your extension.

### Popup.html
The popup.html file is the HTML file for the extension's popup window. You can customize this file as per your needs, adding any HTML, CSS, or JavaScript code required.

### JavaScript and CSS
The js/script.js file is where you can add your own JavaScript code. Similarly, the css/style.css file is where you can add your own CSS styles.

## Webpack

This boilerplate also includes Webpack, a popular module bundler for JavaScript applications. Webpack is used to bundle all the JavaScript code and dependencies into a single file, making it easier to manage and deploy the code.

In this boilerplate, Webpack is configured to take src/index.js as the entry point and output the bundle to content.js. This means that all the JavaScript code written in src/index.js as well as any dependencies imported into that file will be bundled together into a single file called content.js.

By using Webpack, you can take advantage of its features such as code splitting, hot module replacement, and tree shaking to optimize your code and improve the performance of your extension.

To configure Webpack for your own needs, you can edit the webpack.config.js file included in this boilerplate. You can customize the entry point, output file name, and various other settings to suit your specific requirements.

## NPM Scripts

This boilerplate also includes a set of npm scripts that you can use to build and manage your extension. The following scripts are available:

- `npm run build-dev`: Builds the extension in development mode, using Webpack's development settings.
- `npm run build-prod`: Builds the extension in production mode, using Webpack's production settings for code optimization and minification.
- `npm run clean`: Removes the content.js file. All the other files of the extension are not removed.
- `npm run watch`: Starts a Webpack watch process, automatically rebuilding the extension whenever changes are made to the source files.

These scripts provide a convenient way to build and manage your extension, and can be customized to suit your specific needs. You can also add your own scripts to the package.json file to automate other tasks related to your extension development.


## Conclusion
This boilerplate provides a basic structure for creating a Chrome Extension with Manifest 3. It includes the necessary files and folder structure to get started quickly, and you can customize it as per your needs.


