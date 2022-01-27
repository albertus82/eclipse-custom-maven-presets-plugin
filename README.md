Eclipse Custom Maven Presets Plugin
===================================

[![Build](https://github.com/albertus82/eclipse-custom-maven-presets-plugin/actions/workflows/build.yml/badge.svg)](https://github.com/albertus82/eclipse-custom-maven-presets-plugin/actions/workflows/build.yml)

***Add Maven presets in Eclipse "Run As" menu***

## Usage

1. Clone this repository;
2. Edit [`plugin.properties`](plugin.properties) and configure the presets you need (up to 9), e.g.:
   ```properties
   1.enabled=1
   1.class=org.eclipse.m2e.actions.ExecutePomAction:clean package
   1.label=Maven clean package
   ```
4. Launch `./mvnw clean verify`
5. Close **Eclipse** and copy `target/*.jar` to the **Eclipse** `plugins` directory;
6. Restart **Eclipse** with `-clean` option;
7. Select a Maven project or a `pom.xml` file and check the **"Run As"** menu.

### Before:
![before](https://user-images.githubusercontent.com/8672431/151350506-3452a828-1c7e-4c70-96fc-4afa2ff97194.png)

### After:
![after](https://user-images.githubusercontent.com/8672431/151350514-a80822f9-cabd-43d4-a490-e9b9ca0f66d2.png)
