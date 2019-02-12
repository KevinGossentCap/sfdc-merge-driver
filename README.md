sfdc-mergetool
==============

Merge salesforce metadata with ease

[![Version](https://img.shields.io/npm/v/sfdc-mergetool.svg)](https://npmjs.org/package/sfdc-mergetool)
[![CircleCI](https://circleci.com/gh/leboff/sfdc-mergetool/tree/master.svg?style=shield)](https://circleci.com/gh/leboff/sfdc-mergetool/tree/master)
[![Appveyor CI](https://ci.appveyor.com/api/projects/status/github/leboff/sfdc-mergetool?branch=master&svg=true)](https://ci.appveyor.com/project/leboff/sfdc-mergetool/branch/master)
[![Codecov](https://codecov.io/gh/leboff/sfdc-mergetool/branch/master/graph/badge.svg)](https://codecov.io/gh/leboff/sfdc-mergetool)
[![Downloads/week](https://img.shields.io/npm/dw/sfdc-mergetool.svg)](https://npmjs.org/package/sfdc-mergetool)
[![License](https://img.shields.io/npm/l/sfdc-mergetool.svg)](https://github.com/leboff/sfdc-mergetool/blob/master/package.json)

<!-- toc -->
# Usage
<!-- usage -->
### Add Driver to .gitconfig
Add the following lines to your ~/.gitconfig file

```
[merge "sfdcm"]
	name = Merge Driver for Salesforce Metadata
	driver = sfdcm %O %A %B %P
```

### Add merge driver for SFDC metadata types in git attributes
Add the following to your gitattributes file. This can be your `<project-root>/.gitattributes` or `<project-root>/.git/info/attributes` files

```
*.object merge=sfdcm
*.profile merge=sfdcm
*.assignmentRules merge=sfdcm
*.sharingRules merge=sfdcm
*.permissionset merge=sfdcm
*.workflow merge=sfdcm
*.objectTranslations merge=sfdcm
*.translations merge=sfdcm
*.labels merge=sfdcm
*.standardValueSet merge=sfdcm
*.globalValueSet merge=sfdcm
```

# Commands

Test your tool is installed
`sfdcm --version`
