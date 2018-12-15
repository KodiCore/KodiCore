# KodiCore

[![Codacy Badge](https://api.codacy.com/project/badge/Grade/fc6ad96bff994eceb807dc979b2d9bae)](https://www.codacy.com/app/CodeNet/KodiCore?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=Prouser123/KodiCore&amp;utm_campaign=Badge_Grade)
![Build Type - Shields.io](https://img.shields.io/badge/buildtype-maven-red.svg)
![Lines of Code](https://tokei.rs/b1/github/Prouser123/KodiCore)

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

## Key Methods

More (and detailed) information for all methods can be found in the documentation, linked below.

[FULL Documentation Link](https://kodicore.github.io/KodiCore)

### Console

KodiCore Console Logging - log to the console with info, warning or severe types.

**Class Location:** [me.prouser123.kodicore.send.Console](https://kodicore.github.io/KodiCore/me/prouser123/kodicore/send/Console.html)

**Required for plugin operation?** Yes

**Requires new instance?** Yes - create with `new Console(this);` from your plugin's Main class.

### Chat

**Class Location:** [me.prouser123.kodicore.send.Chat](https://kodicore.github.io/KodiCore/me/prouser123/kodicore/send/Chat.html)

**Requires new instance?** No, just import the class and start coding!

Features:
- Chat to permission
- Chat to player
- Chat to players
- Chat to server / Broadcast to server
- Chat to world

### Utils

**Class Location:** [me.prouser123.kodicore.Utils](https://kodicore.github.io/KodiCore/me/prouser123/kodicore/Utils.html)

**Requires new instance?** No, just import the class and start coding!

Features:
- Add item to inventory (with modifiers)
- Run a command in the console
- Get World (by name)
- Broadcasting
- getConfig getInt
- getConfig getString
- Get online players (amount)
- Get online players (player names)
 
### Discord

**Class Location:** 
[me.prouser123.kodicore.Discord](https://kodicore-4vjczy4tx.now.sh/docs/me/prouser123/kodicore/discord/Discord.html)

**Requires new instance?** Yes. Create with `new Discord("discord-bot-token");`

After you have created a instance you can add various things to your bot. See the docs for details.


Example feature:

- Discord `!serverinfo` command

  Use `Discord.api.addMessageCreateListener(new ServerInfo());` to enable.

  Example output:

  <img src="https://github.com/KodiCore/DiscordBot/raw/master-standalone/serverinfo_output.PNG" alt="Output" width=550>
