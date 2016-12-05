# Iguana Desktop App
Desktop App for SuperNET DAPPs

#### For Developers
You must have `node.js` and `npm` installed on your machine.

Clone Iguana Desktop App
```shell
git clone https://github.com/SuperNETorg/iguana.git
```

Please clone EasyDEX-GUI from github repo here.
```shell
mkdir gui
cd gui
git clone https://github.com/SuperNETorg/EasyDEX-GUI.git
```

Install Iguana App
```shell
cd iguana
npm install
```

Then start Iguana App
```shell
npm start
```

#### For end users
The instructions to make production build of Iguana App will be updated soon.

To build the production ready app, install `electron-packager` and `electron-prebuilt` packages from npm
```shell
npm install electron-packager -g
npm install electron-prebuilt -g
```

#### **Build the Wallet-App**
Refer to the original [electron-packager](https://github.com/electron-userland/electron-packager) repository for more detailed information.

##### Linux
Change directory to iguana and execute the following command to build the Linux app
```shell
cd iguana
electron-packager . --platform=linux --arch=ia32 --out=build/
```
change architecture build parameter to ```--arch=x64``` for 64 bit build

##### OSX
Change directory to iguana and execute the following command to build the OSX app
```shell
cd iguana
electron-packager . --platform=darwin --arch=x64 --icon=assets/icons/komodo.icns --out=build/
```

##### Windows
Change directory to iguana and execute the following command to build the Windows app
```shell
dir iguana
electron-packager . --platform=win32 --arch=ia32 --icon=assets/icons/komodo.ico --out=build/
```
change architecture build parameter to ```--arch=x64``` for 64 bit build