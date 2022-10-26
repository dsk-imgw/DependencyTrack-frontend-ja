# dependency-track-ja

This project is a Japanese translation effort of [Dependency-Track Frontend](https://github.com/DependencyTrack/frontend).
Basically, "en.json", which is provided by Dependency-Track Frontend, is translated into Japanese as a file "ja.json",
and some files are modified in order to switch locales.

*NOTE: This project has nothing to do with the original [Dependency-Track](https://dependencytrack.org/).*

# How To Use

1. Download a source code of [Dependency-Track Frontend](https://github.com/DependencyTrack/frontend) (*1) which is compatible with Dependency-Track API server you are using.
2. Download a source code on this repository (*2) the version of which matches that of Dependency-Track Frontend.
3. Unzip (*1), then unzip (*2) with overwriting (*1).
4. Open a terminal and type the following commands.
```
$ cd /path/to/Dependency-Track Frontend/
$ npm install
$ npm audit fix
$ npm run build
```
5. If the command ```npm run build``` is successful, then edit properly a file ```dist/static/config.json``` (, or delete it).
6. Copy the files and directories under ```dist/``` to the document root of Dependency-Track Frontend server.
7. Set your browser's preffered language to the locale you want to use, and access Dependency-Track Frontend server.

![Dependency-Track_Dashboard_ja](https://user-images.githubusercontent.com/100552204/174016314-3b4dfc38-83c4-4b82-8f93-1b5d6dd8697e.png)
