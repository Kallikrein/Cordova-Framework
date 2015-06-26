# Cordova-Framework

## Summary
* [Files architecture](#files-architecture)
* [Cordova](#cordova)

-----

#### Files architecture

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
