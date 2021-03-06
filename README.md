# Sirius Development Kit

[![Build Status](https://travis-ci.com/pcdavid/sirius-kit.svg?branch=master)](https://travis-ci.com/pcdavid/sirius-kit)

Defines a simple feature with all the tools needed to develop/contribute to [Eclipse Sirius](https://www.eclipse.org/). Designed to be installed on top of a plain [Eclipse IDE for Eclipse Committers](https://www.eclipse.org/downloads/packages/release/2018-09/r/eclipse-ide-eclipse-committers) package.

Note that this is not (yet) offically part of Eclipse Sirius but just provided here as a convenience.

## Content

The feature `org.eclipse.sirius.tools.kit` includes the following components:
* Acceleo 2.8 (needed for the legacy code generation step for the VSM editor's property sections).
* Acceleo 3.7, used by some of our examples.
* Target Platform DSL 3.0.0-SNAPSHOT from [Eclipse CBI](https://github.com/eclipse-cbi/). Note that this is using a (moving) snapshot build at the moment.
* EMF SDK 2.16.0 from Eclipse 2018-12.
* SWTBot IDE Integration 2.8-m3, needed to launch our automated SWTBot tests.
* Eclipse FindBugs plug-in 3.0.1. Not strictly needed, and may be replaced by [SpotBugs](https://spotbugs.github.io/) at some point.
* Eclipse CheckStyle Plug-in 8.12.0.
* Mylyn WikiText Editor 3.0.25 (the version from Eclipse 2018-09), as a convenience to edit various Textile and Markdown documents (notable the Sirius documentation).
* Eclipse XML Editors and Tools (the version from Eclipse 2018-09) to edit various XML files more comfortably.

## Build

To build it yourself, simply clone the repo and from the top-level directory issue

```
mvn clean package
```

The resulting p2 repository is located in `org.eclipse.sirius.tools.kit-repo/target`.

## License

Copyright (c) 2018 Obeo.

This program and the accompanying materials are made available under the terms of the Eclipse Public License 2.0 which accompanies this distribution, and is available at https://www.eclipse.org/legal/epl-2.0/
