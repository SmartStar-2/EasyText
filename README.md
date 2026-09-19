# 🌈 EasyText

**EasyText** is a powerful text-formatting plugin for Minecraft Paper servers.

It replaces complicated formatting with simple and memorable `@` codes.

Instead of dealing with traditional formatting codes, simply write:

```text
@rHello!
```

EasyText turns the text into formatted Minecraft text.

Combine multiple codes to create more advanced styles:

```text
@r@fe3Hello!
@re@fe5Rainbow!
@pi@kuHello!
```

---

# 📦 Requirements

- **Minecraft / Paper:** 26.2
- **Java:** 25
- **EasyText version:** 1.0.0
- **Additional plugins:** None required

EasyText has been successfully loaded and enabled on a real Paper 26.2 server.

---

# ✨ Features

EasyText includes:

- 🎨 Standard Minecraft colors
- 🌈 Rainbow text
- 🌈 Reverse rainbow text
- 🎲 Random colors
- 🔄 Alternating colors
- 🎨 Custom RGB/HEX colors
- **Bold formatting**
- *Italic formatting*
- Obfuscated / magic text
- Formatting reset
- Book formatting
- Sign formatting
- Anvil formatting
- Item-name formatting
- Formatting preview
- Optional chat formatting
- Built-in help
- Roles
- Per-player permissions
- ALLOW / DENY / INHERIT permission states
- Configurable modules
- Admin GUI
- Owner claim system
- Persistent configuration

---

# 🎨 Color Codes

## Standard Colors

| Code | Color |
|---|---|
| `@r` | Red |
| `@ge` | Yellow |
| `@bl` | Blue |
| `@gr` | Green |
| `@aq` | Aqua |
| `@li` | Purple |
| `@pi` | Pink |
| `@go` | Gold |
| `@w` | White |
| `@sw` | Black |
| `@dr` | Dark Red |
| `@db` | Dark Blue |
| `@dg` | Dark Green |
| `@hg` | Light Gray |
| `@gg` | Dark Gray |

Example:

```text
@rThis text is red!
```

---

# 🌈 Special Colors

## Rainbow

```text
@reHello World!
```

Creates rainbow-colored text.

## Reverse Rainbow

```text
@rvHello World!
```

Creates a rainbow in the opposite direction.

## Random Colors

```text
@zuHello World!
```

Applies randomized colors.

## Alternating Colors

```text
@wbHello World!
```

Creates alternating/ changing colors.

---

# 🎨 Custom HEX Colors

EasyText supports custom RGB/HEX colors.

Format:

```text
@#RRGGBB
```

Example:

```text
@#FF8800Hello!
```

This allows you to use colors beyond Minecraft's standard color palette.

---

# ✍️ Text Styles

## Italic

```text
@kuHello!
```

## Obfuscated / Magic Text

```text
@obHello!
```

## Bold Levels

EasyText provides:

```text
@fe1
@fe2
@fe3
@fe4
@fe5
```

Example:

```text
@fe3Hello!
```

Minecraft itself only has one native bold weight. EasyText's multiple bold levels are therefore simulated rather than five separate native Minecraft font weights.

---

# 🔄 Reset Formatting

Use:

```text
@rs
```

to reset active formatting.

Example:

```text
@rRed text @rsNormal text
```

---

# @️⃣ Writing a Real @ Symbol

Because EasyText uses `@` to start formatting codes, use:

```text
@@
```

when you want an actual `@` character.

Example:

```text
Contact @@Vinchi999
```

---

# 🔗 Combining Formatting

Formatting codes can be combined.

Examples:

```text
@r@fe3Hello!
```

Red + bold formatting.

```text
@re@fe5Rainbow!
```

Rainbow + bold formatting.

```text
@pi@kuHello!
```

Pink + italic.

A new color replaces the previous active color while compatible text effects can remain active until they are reset.

---

# 📖 Books

EasyText supports formatting in books.

Formatting is applied when supported book content is finalized/saved by the plugin.

Example:

```text
@reWelcome to our server!
```

---

# 🪧 Signs

EasyText can format supported sign text.

Example:

```text
@goSHOP
```

---

# ⚒️ Anvils

EasyText supports formatted item names through anvils when the Anvil module and the player's permissions allow it.

Example name:

```text
@reLegendary Sword
```

---

# 🗡️ Item Names

EasyText can format item names.

The plugin also provides `/fmt` functionality for supported item-name operations.

---

# 💬 Chat Formatting

Chat formatting is optional and can be disabled by the server administrator.

When enabled, supported EasyText codes can be used in chat according to the player's permissions.

Chat formatting is disabled by default in EasyText 1.0.0.

---

# ❓ Help

Use:

```text
/fmt help
```

to access EasyText's built-in help.

The special help code is:

```text
@h
```

where supported by the configured module.

---

# 🖥️ Admin GUI

EasyText includes an administration GUI.

Open it with:

```text
/fmt gui
```

The GUI is designed to help administrators manage EasyText settings such as modules, roles and player permissions.

---

# 👑 Owner Setup

When EasyText starts for the first time, no Owner exists.

The server console generates a temporary claim code.

The console will show something similar to:

```text
MCFormat: Es gibt noch keinen Owner!
Claim-Code: YOUR-CODE
Im Spiel eingeben: /fmt claim YOUR-CODE
```

The player who should own/manage the EasyText installation can then use:

```text
/fmt claim <code>
```

Alternatively, the server console supports assigning the Owner role using the plugin's role command.

**Keep your claim code private.**

---

# 👥 Roles

EasyText contains four main roles:

| Role | Purpose |
|---|---|
| **Owner** | Full control over EasyText |
| **Admin** | Administrative management |
| **Moderator** | Limited moderation/management |
| **Player** | Normal user |

The Owner has the highest level of EasyText access.

EasyText also includes protections intended to prevent users from granting themselves privileges they should not have.

---

# 🔐 Permission System

EasyText includes its own detailed permission system.

A player permission can have three states:

### ALLOW

Explicitly allows the feature.

### DENY

Explicitly blocks the feature.

### INHERIT

Uses the permission inherited from the player's role/default configuration.

---

# 🛡️ Permission Priority

EasyText's permission system is designed around a priority model.

The general structure is:

1. Owner access
2. Explicit player DENY
3. Explicit player ALLOW
4. Role permissions
5. Default permissions
6. Deny when no permission grants access

An administrator can therefore give individual players access to specific EasyText features without granting full administrative access.

---

# 🔑 Feature Permissions

EasyText separates permissions by feature.

Examples include:

```text
format.books
format.anvil
format.colors
format.rainbow
format.bold
```

Administrative permission areas include functionality such as:

```text
admin.config
admin.roles
admin.permissions
```

The exact permission configuration used by your server can be viewed and managed through EasyText's administration system.

---

# 🧩 Modules

EasyText is modular.

Server administrators can independently control functionality such as:

```text
books
anvil
itemNames
signs
colors
rainbow
reverseRainbow
randomColors
alternatingColors
bold
italic
obfuscated
help
```

A disabled module prevents that feature from being used even when a player would otherwise have permission to use it.

This allows server owners to enable only the EasyText functionality they want.

---

# 👤 Default Player Access

EasyText uses restrictive defaults for advanced functionality.

Normal players do not automatically receive every EasyText feature.

Server administrators can grant additional functionality using EasyText's permission system.

For example, access to features such as anvils, signs or rainbow formatting can be controlled separately.

---

# 🧰 Commands

The primary command is:

```text
/fmt
```

Important confirmed EasyText commands include:

| Command | Description |
|---|---|
| `/fmt help` | Shows EasyText help |
| `/fmt gui` | Opens the administration GUI |
| `/fmt claim <code>` | Claims the initial Owner role |
| `/fmt name ...` | Item-name formatting functionality |

EasyText also contains administrative functionality for managing roles, permissions and configuration.

For the exact command syntax available on your installed version, use:

```text
/fmt help
```

This is recommended because available commands can depend on your role, permissions and enabled modules.

---

# 💾 Persistent Settings

EasyText saves its configuration so settings can survive server restarts.

This includes the plugin's management information required for its roles, permissions and configurable functionality.

---

# ⚙️ How Permissions and Modules Work Together

Having permission does **not** automatically override a disabled module.

For example:

```text
Player has: format.rainbow = ALLOW
Rainbow module = OFF
```

Result:

```text
Rainbow formatting is unavailable.
```

The module switch has priority over access to that feature.

---

# 📝 Formatting Examples

### Red

```text
@rHello!
```

### Green

```text
@grHello!
```

### Gold

```text
@goHello!
```

### Rainbow

```text
@reHello!
```

### Reverse Rainbow

```text
@rvHello!
```

### Italic Pink

```text
@pi@kuHello!
```

### Rainbow + Bold

```text
@re@fe5Hello!
```

### Custom Orange

```text
@#FF8800Hello!
```

### Reset

```text
@rRed @rsNormal
```

### Literal @

```text
@@Vinchi999
```

---

# ⚠️ Important Notes

## Bold Levels

Minecraft does not provide five separate native bold weights.

EasyText therefore simulates the `@fe1`–`@fe5` levels.

## Books

Minecraft has technical limitations regarding formatted editable book content. EasyText applies book formatting at the appropriate supported stage.

## Owner Detection

A Paper plugin cannot simply assume which Minecraft player is the actual human owner of a hosted server.

For this reason, EasyText uses its Owner claim system during initial setup.

---

# 🚀 Installation

1. Download `MCFormat-1.0.0.jar`.
2. Stop your Paper server.
3. Place the JAR inside:

```text
plugins/
```

4. Start the server.
5. Check the console for the EasyText/MCFormat startup message.
6. Complete the Owner setup if this is the first launch.
7. Run:

```text
/fmt help
```

EasyText should now be ready.

---

# ✅ Tested Environment

EasyText 1.0.0 has been loaded successfully with:

- **Paper 26.2**
- **Java 25**

The server successfully recognized and enabled:

```text
MCFormat v1.0.0
```

without an MCFormat startup exception during the tested server launch.

Individual server configurations and plugin combinations can still affect behavior, so testing EasyText on your server before using it in production is recommended.

---

# 🐛 Found a Bug?

If something does not work correctly, please include:

- EasyText version
- Paper version
- Java version
- What you were trying to do
- What happened instead
- Relevant console error/log
- Steps to reproduce the problem

Please **never include passwords, API keys, server login details or other private information** in a public bug report.

---

# 📋 Version

## EasyText 1.0.0

Initial public release.

Main features include advanced `@` formatting, colors, rainbow effects, books, signs, item names, role management, granular permissions and administrative configuration.

---

# ❤️ EasyText

EasyText was created to make advanced Minecraft text formatting easier to use and easier for server administrators to control.

**Simple codes. Powerful formatting.**
