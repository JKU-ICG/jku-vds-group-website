---
layout: documentation
title:  Caleydo Directory Structure
permalink: /documentation/directory_structure/
description: Explains the basic directory structure
---

After the installation you find the following basic directory structure:

```
caleydo_web_container
+---.tscache
+---.vagrant
+---_data
+---_idea_template
+---libs
|   \---bower_components
+---node_modules
+---plugins
|   |---caleydo_core
|   \---...
+---scripts
+---static
+---typings
```


* `caleydo_web_container` the cloned [caleydo_web_container repository](https://github.com/Caleydo/caleydo_web_container) as root directory
* `.tscache` the working directory of the TypeScript compiler
* `.vagrant` the working directory of [Vagrant](https://www.vagrantup.com/)
* `_data` shared data directory for all plugins
* `_idea_template` settings and template for [JetBrains PyCharm](https://www.jetbrains.com/pycharm/)
* `libs` external libraries
   * `bower_components` resolved [bower dependencies](http://bower.io/)
* `node_modules` resolved [node modules](https://www.npmjs.com/) (for *Windows* this is just a symbolic link into the vagrant machine)
* `plugins` all available plugins (e.g., using the `./manage.sh clone` command)
   * `caleydo_core`
   * other plugins
* `scripts` shell scripts for Caleydo internal usage
* `static` static files that are used as web root; some are generated by Caleydo
* `typings` the resolved [TypeScript definitions](http://definitelytyped.org/) to provide auto-complete and type checking for external libraries
