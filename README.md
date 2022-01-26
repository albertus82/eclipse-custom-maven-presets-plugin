Eclipse Custom Maven Presets Plugin
===================================

[![Build](https://github.com/albertus82/eclipse-custom-maven-presets-plugin/actions/workflows/build.yml/badge.svg)](https://github.com/albertus82/eclipse-custom-maven-presets-plugin/actions/workflows/build.yml)

***Add Maven presets in Eclipse "Run As..." context menu***

## Usage

1. Clone this repository
2. Edit `plugin.properties` and configure the presets you need (up to 9)
3. Launch `mvnw clean verify`
4. Copy `target/*.jar` to the `plugins` directory of **Eclipse**
5. Start **Eclipse** with `-clean` option
6. Right click on a Maven project or a `pom.xml` file and check the **Run As...** context menu
