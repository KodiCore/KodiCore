# KodiCore

[![Codacy Badge](https://api.codacy.com/project/badge/Grade/b000a83e48c142b2870cf4fe46b36c14)](https://www.codacy.com/app/KodiCore/KodiCore?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=KodiCore/KodiCore&amp;utm_campaign=Badge_Grade)
[![TravisCI Build Status](https://travis-ci.com/KodiCore/KodiCore.svg?branch=master)](https://travis-ci.com/KodiCore/KodiCore)
![Build Type - Shields.io](https://img.shields.io/badge/type-maven-red.svg)
![Lines of Code](https://tokei.rs/b1/github/KodiCore/KodiCore)

A set of functions to make plugin debugging and development easier.

## Setup (Maven)
Add this to the `repositories` section of your `pom.xml`:
```xml
<repositories>
  <!-- KodiCore -->
  <repository>
    <id>Prouser123-kodi-core</id>
    <url>https://packagecloud.io/Prouser123/kodi-core/maven2</url>
    <releases>
      <enabled>true</enabled>
    </releases>
    <snapshots>
      <enabled>true</enabled>
    </snapshots>
  </repository>
</repositories>
```

Then add this to the `dependencies` section of your `pom.xml`:
```xml
<dependencies>
  <!-- KodiCore -->
  <dependency>
    <groupId>me.prouser123</groupId>
    <artifactId>kodicore</artifactId>
    <version>LATEST</version>
    <scope>provided</scope>
  </dependency>
</dependencies>
```
