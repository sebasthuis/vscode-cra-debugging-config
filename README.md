# VSCode debugger config for Create React App applications

This repository provides VSCode configuration that allows for easy debugging
within the editor/IDE for Create React App (CRA) web applications. By default it
debugs applications in Chrome, but it is easy to setup different browsers.

The configuration is setup to mimick the style of debugging of Visual Studio
XXXX. Where starting the debugging will spin up all required processes and will
quit the processes once the debugging is stopped.

## Assumptions

1. The application runs on port 3000.
2. There is a `start` script in the package.json.

```json
"scripts": {
    "start": "react-scripts start"
}
```

3. The `BROWSER=none` environment value is able to suppress the start script
   from opening a browser or tab.

## How to Use

1. Copy the contents of the `.vscode` directory into the root of your
   repository, create the directory if the folder does not exist. In the case of
   existing configuration files, please merge the contents.

2. Start debugging either by pressing `F5` or navigating to the `Run and Debug`
   panel in VSCode and selecting `Launch Chrome against localhost` and pressing the
   green play button at the top of the panel.

3. After debugging press the `Stop` button of the debugging menu or close the
   new instance of Chrome that was opened in the process.
