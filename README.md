# Website

This website is built using [Docusaurus](https://docusaurus.io/), a modern static website generator.

### Installation

First you will need to install [Node.js](https://nodejs.org/en/download/)

Next make sure your execution policy is set so that scripts can run if you are running this on a normal Windows machine.
To do this open Powershell as Administrator and use the following comand:
```
Set-ExecutionPolicy
```
It will ask what policy you want to set. Enter `RemoteSigned` and then enter `A` to say yes to all security prompts. After that you should be able to run the development environment and build command.

Next you need to install Docusaurus. Where you install it does not matter as we will be moving it after the install. Hold [Shift] and right-click in the temp directory you wish to install Docusaurus in, then run the following command:

```
npx create-docusaurus@latest my-website classic
```

When prompted to select `JavaScript` and let the installer run.

Once the install is completed close Powershell and navigate to the `my-website` folder it created.

You can then move the `.docusaurus`, `node_modules` folders to the repository folder.

After you move those two folders you can delete the `my-website` folder.

### Local Development

To start the development environment navigate to the repositoty folder using File Explorer or ``cd``. Then run the following command:

```
npx docusaurus start
```

This command starts a local development server and opens up a browser window. Most changes are reflected live without having to restart the server.

### Build

```
npx docusaurus build
```

This command generates static content into the `build` directory where it then can be deployed to the webserver.

### Updating

Check current version of Docusaurus:

```
npx docusaurus --version
```

Update Docusaurus:

```
npx install
```

*(Make sure you are running these commands inside the repositoty directory where `package.json` is located.)*
