# Cordova-Framework

## Summary
* [Installation](#installation)
* [Troubleshooting](#troubleshooting)
* [Files architecture](#files-architecture)
* [Cordova](#cordova)

-----

### installation

```
git clone https://github.com/Kallikrein/Cordova-Framework.git
cd Cordova-Framework
./install.sh
source .aliases
```  
> If you have a boot2docker VM running on windows you need to source also :
```
source .boot2docker_aliases
```

```
cd cordova
cordova platform add android
```

> For this version, you need to install bower components. See more [here](https://github.com/Kallikrein/core/blob/master/README.md).
```
cd core
bower install
cd ..
```

```
cordova build
```

> If you have an android device recognised :

```cordova run```

### troubleshooting

boot2docker :
- if you are using virtual box (by default with boot2docker), you need to configure virtual box to allow symlinks :  
```VBoxManage setextradata VM_NAME VBoxInternal2/SharedFoldersEnableSymlinksCreate/SHARE_NAME 1```  
- if you have an android device you need to share the usb to the vm
SEE SCREEN CAPTURE
- deactivate hyperV
TODO SCREEN CAPTURE
- VTx activated in bios
CHECK IF OPTION IS ACTIVE IN VIRTUAL BOX

### Files architecture

<pre>
<b>./</b>
├── <b><a href="#cordova">cordova/</a></b>
|   ├── <b><a href="#core">core/</a></b>
|   ├── <b><a href="#hooks">hooks/</a></b>
|   ├── <b><a href="#instance">instance/</a></b>
|   ├── <b><a href="#platforms">platforms/</a></b>
|   ├── <b><a href="#plugins">plugins/</a></b>
|   ├── <a href="#config">config.xml</a>
|   └── <b><a href="#www">www/</a></b>
├── <a href="#aliases">.aliases</a>
├── <a href="#boot2docker">.boot2docker_aliases/</a>
├── <a href="#gitignore">.gitignore</a>
├── <a href="#readme">README.md</a>
└── <a href="#install">install.sh</a>
</pre>

#### cordova/
> [Cordova v5.1.1](http://cordova.apache.org/docs/en/5.1.1/index.html)

**Cordova** is a platform for building native mobile applications using HTML, CSS and Javascript on all the most popular mobile OS. It creates a WebView component where your code is executed and provides an interface that let you call native function in Javascript.
This is where all **cordova** files are stored to build mobile application.<br>
