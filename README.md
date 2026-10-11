<picture>
  <source media="(prefers-color-scheme: dark)" srcset="assets/banner-dark.svg">
  <source media="(prefers-color-scheme: light)" srcset="assets/banner-light.svg">
  <img src="assets/banner-dark.svg" width="100%" alt="Matt Bäumli. Application Owner, AI Tooling Developer, Ex-Chef, Videogame Purist, Dog Person">
</picture>

<p align="center"><i>AI made code cheap. Understanding the system still isn't.</i></p>

I cooked professionally for years before I traded the knives for an editor. In 2026 I finished my apprenticeship as an application developer (Informatiker EFZ) with an award for my final grade. Today I'm Application Owner at TESTEX, where I also write the handlers and parsers that connect our lab instruments to LabVantage LIMS.

In summer 2027 I start at a Swiss college of higher education (HF). The long-term goal is AI and machine learning, and I pick up everything useful on the way. Claude is my daily sparring partner for design decisions, research and long technical arguments. I use it to think, not to skip thinking.

## <img src="assets/icons/featured.svg" width="20" height="20" alt=""> Featured

### Smart Ticket Helper
<sub>Final project (IPA) 2026 · internal at TESTEX, not public</sub>

A support agent types a problem in their own words and gets the closest matches from three years of support history, even when the old ticket is in Chinese and the question is in German. The old search only knew exact keywords.

Embeddings and search run entirely on-premise, so in production no ticket data goes to an outside service. The tool retrieves real tickets instead of generating text, which means it can't make anything up. When nothing fits, it says so.

Two things no tutorial prepared me for. The textbook similarity threshold rejected every single correct match, so I calibrated my own on real tickets. And the GPU turned embeddings into NaN, so inference moved to the CPU, where it ran faster anyway.

`Python` `FastAPI` `PostgreSQL` `pgvector` `Ollama`

### [GlyphKit](https://github.com/Lunyxium/glyphkit)
<sub>Windows · open source (GPL-3.0)</sub>

A floating Unicode palette that never steals focus. Click `∑` and it lands right where you were typing. I built it because Windows makes you dig through the character map for every single symbol. One portable .exe, zero dependencies, Win32 called straight from Python.

`Python` `Win32` `tkinter`

### [HexColorPicker](https://github.com/Lunyxium/HexColorPicker)
<sub>Windows · open source (MIT)</sub>

A small hex color picker, because I was tired of opening a browser for a color code. Pick by hue, saturation and brightness, copy the hex with or without `#`.

`C#` `WPF` `.NET`

## <img src="assets/icons/private.svg" width="20" height="20" alt=""> Building in private

<sub>No public repos yet. Click a project for details.</sub>

<details>
<summary><b>Claude Code mods</b> · Claude Code, steered from a UI instead of slash commands</summary>
<br>

A HUD above the chat input and a side pane show what every agent is doing, how far the current task has come, where the usage limits stand and what the session would have cost at API prices. One panel switches skills, hooks and agent behavior on for the next prompt, the whole session or globally, without touching a JSON file. An editor for Claude's config files is in progress.

The stock UI components weren't enough, so I wrote a skill on custom buttons, menus, panes and CSS for mods. My agents now use it to build the rest. There's also a radio. And a customizable Claude pet.

<sub>Catalog coming to GitHub soon.</sub>

</details>

<details>
<summary><b>EonHeart</b> · a browser MMO whose game logic lives inside the database</summary>
<br>

Built in Godot for the web. The game logic lives inside SpacetimeDB as server modules, and clients subscribe straight to the world state. No separate game server, no hand-written netcode, so the time goes into the game instead of the plumbing.

`Godot` `SpacetimeDB`

</details>

<details>
<summary><b>Untitled drawing app</b> · drawing with an AI on the same canvas</summary>
<br>

Pin notes to exact spots on any layer, sketch the line you want on a layer of its own, and the AI, connected over MCP, sees exactly what you mean and can mark up the image in return. Made for my own game and 3D art workflow.

</details>

<details>
<summary><b>Vivarium</b> · any website as its own isolated desktop app</summary>
<br>

Turns any website into a real desktop app with its own isolated session, window, Start Menu shortcut and taskbar entry. Install YouTube twice, once for work and once for yourself, logged into different accounts, and the two never see each other. Private mode forgets everything when the window closes. No account, no telemetry.

<sub>Windows · on pause, not abandoned</sub>

`Electron` `React` `TypeScript` `Tailwind`

</details>

## <img src="assets/icons/stack.svg" width="20" height="20" alt=""> Stack

**Favourites**<br>
<img width="134" src="https://img.shields.io/badge/Python-1a1816?style=flat-square&logo=python&logoColor=2dd4bf" alt="Python"> <img width="170" src="https://img.shields.io/badge/JavaScript-1a1816?style=flat-square&logo=javascript&logoColor=2dd4bf" alt="JavaScript"> <img width="174" src="https://img.shields.io/badge/TypeScript-1a1816?style=flat-square&logo=typescript&logoColor=2dd4bf" alt="TypeScript"> <img width="90" src="https://img.shields.io/badge/C%23-1a1816?style=flat-square&logo=data:image%2Fsvg%2Bxml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHZpZXdCb3g9IjAgMCAyNCAyNCI%2BPHBhdGggZD0iTTEzLjUgNy42QTYgNiAwIDEgMCAxMy41IDE2LjQiIGZpbGw9Im5vbmUiIHN0cm9rZT0iIzJkZDRiZiIgc3Ryb2tlLXdpZHRoPSIyIiBzdHJva2UtbGluZWNhcD0icm91bmQiIHN0cm9rZS1saW5lam9pbj0icm91bmQiLz48cGF0aCBkPSJNMTYuMiA4LjUgMTUuNiAxNS41TTE5LjYgOC41IDE5IDE1LjVNMTQuNiAxMC42SDIxTTE0LjQgMTMuNEgyMC44IiBmaWxsPSJub25lIiBzdHJva2U9IiMyZGQ0YmYiIHN0cm9rZS13aWR0aD0iMiIgc3Ryb2tlLWxpbmVjYXA9InJvdW5kIiBzdHJva2UtbGluZWpvaW49InJvdW5kIi8%2BPC9zdmc%2B" alt="C#">

**AI & data**<br>
<img width="130" src="https://img.shields.io/badge/Claude-1a1816?style=flat-square&logo=claude&logoColor=2dd4bf" alt="Claude"> <img width="194" src="https://img.shields.io/badge/Claude_Code-1a1816?style=flat-square&logo=claude&logoColor=2dd4bf" alt="Claude Code"> <img width="102" src="https://img.shields.io/badge/MCP-1a1816?style=flat-square&logo=modelcontextprotocol&logoColor=2dd4bf" alt="MCP"><br>
<img width="134" src="https://img.shields.io/badge/Ollama-1a1816?style=flat-square&logo=ollama&logoColor=2dd4bf" alt="Ollama"> <img width="182" src="https://img.shields.io/badge/PostgreSQL-1a1816?style=flat-square&logo=postgresql&logoColor=2dd4bf" alt="PostgreSQL"> <img width="154" src="https://img.shields.io/badge/pgvector-1a1816?style=flat-square&logo=postgresql&logoColor=2dd4bf" alt="pgvector">

**Building with**<br>
<img width="138" src="https://img.shields.io/badge/FastAPI-1a1816?style=flat-square&logo=fastapi&logoColor=2dd4bf" alt="FastAPI"> <img width="202" src="https://img.shields.io/badge/SpacetimeDB-1a1816?style=flat-square&logo=data:image%2Fsvg%2Bxml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHZpZXdCb3g9IjAgMCAyNCAyNCI%2BPGVsbGlwc2UgY3g9IjEyIiBjeT0iNiIgcng9IjciIHJ5PSIyLjYiIGZpbGw9Im5vbmUiIHN0cm9rZT0iIzJkZDRiZiIgc3Ryb2tlLXdpZHRoPSIyIiBzdHJva2UtbGluZWNhcD0icm91bmQiIHN0cm9rZS1saW5lam9pbj0icm91bmQiLz48cGF0aCBkPSJNNSA2djEyYzAgMS40IDMuMSAyLjYgNyAyLjZzNy0xLjIgNy0yLjZWNk01IDEyYzAgMS40IDMuMSAyLjYgNyAyLjZzNy0xLjIgNy0yLjYiIGZpbGw9Im5vbmUiIHN0cm9rZT0iIzJkZDRiZiIgc3Ryb2tlLXdpZHRoPSIyIiBzdHJva2UtbGluZWNhcD0icm91bmQiIHN0cm9rZS1saW5lam9pbj0icm91bmQiLz48L3N2Zz4%3D" alt="SpacetimeDB"> <img width="122" src="https://img.shields.io/badge/Godot-1a1816?style=flat-square&logo=godotengine&logoColor=2dd4bf" alt="Godot"> <img width="146" src="https://img.shields.io/badge/Electron-1a1816?style=flat-square&logo=electron&logoColor=2dd4bf" alt="Electron"><br>
<img width="118" src="https://img.shields.io/badge/React-1a1816?style=flat-square&logo=react&logoColor=2dd4bf" alt="React"> <img width="146" src="https://img.shields.io/badge/Tailwind-1a1816?style=flat-square&logo=tailwindcss&logoColor=2dd4bf" alt="Tailwind"> <img width="246" src="https://img.shields.io/badge/Azure_Logic_Apps-1a1816?style=flat-square&logo=data:image%2Fsvg%2Bxml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHZpZXdCb3g9IjAgMCAyNCAyNCI%2BPHJlY3QgeD0iMi41IiB5PSIzIiB3aWR0aD0iNiIgaGVpZ2h0PSI2IiByeD0iMS41IiBmaWxsPSJub25lIiBzdHJva2U9IiMyZGQ0YmYiIHN0cm9rZS13aWR0aD0iMiIgc3Ryb2tlLWxpbmVjYXA9InJvdW5kIiBzdHJva2UtbGluZWpvaW49InJvdW5kIi8%2BPHJlY3QgeD0iMTUuNSIgeT0iMyIgd2lkdGg9IjYiIGhlaWdodD0iNiIgcng9IjEuNSIgZmlsbD0ibm9uZSIgc3Ryb2tlPSIjMmRkNGJmIiBzdHJva2Utd2lkdGg9IjIiIHN0cm9rZS1saW5lY2FwPSJyb3VuZCIgc3Ryb2tlLWxpbmVqb2luPSJyb3VuZCIvPjxyZWN0IHg9IjkiIHk9IjE1IiB3aWR0aD0iNiIgaGVpZ2h0PSI2IiByeD0iMS41IiBmaWxsPSJub25lIiBzdHJva2U9IiMyZGQ0YmYiIHN0cm9rZS13aWR0aD0iMiIgc3Ryb2tlLWxpbmVjYXA9InJvdW5kIiBzdHJva2UtbGluZWpvaW49InJvdW5kIi8%2BPHBhdGggZD0iTTguNSA2aDdNMTguNSA5YzAgNC02LjUgMi41LTYuNSA2IiBmaWxsPSJub25lIiBzdHJva2U9IiMyZGQ0YmYiIHN0cm9rZS13aWR0aD0iMiIgc3Ryb2tlLWxpbmVjYXA9InJvdW5kIiBzdHJva2UtbGluZWpvaW49InJvdW5kIi8%2BPC9zdmc%2B" alt="Azure Logic Apps">

**Worked with**<br>
<img width="106" src="https://img.shields.io/badge/Java-1a1816?style=flat-square&logo=openjdk&logoColor=2dd4bf" alt="Java"> <img width="106" src="https://img.shields.io/badge/C%2B%2B-1a1816?style=flat-square&logo=cplusplus&logoColor=2dd4bf" alt="C++"> <img width="194" src="https://img.shields.io/badge/React_Native-1a1816?style=flat-square&logo=react&logoColor=2dd4bf" alt="React Native"> <img width="162" src="https://img.shields.io/badge/MongoDB-1a1816?style=flat-square&logo=mongodb&logoColor=2dd4bf" alt="MongoDB"><br>
<img width="134" src="https://img.shields.io/badge/Docker-1a1816?style=flat-square&logo=docker&logoColor=2dd4bf" alt="Docker"> <img width="150" src="https://img.shields.io/badge/Firebase-1a1816?style=flat-square&logo=firebase&logoColor=2dd4bf" alt="Firebase"> <img width="86" src="https://img.shields.io/badge/Git-1a1816?style=flat-square&logo=git&logoColor=2dd4bf" alt="Git"> <img width="130" src="https://img.shields.io/badge/GitHub-1a1816?style=flat-square&logo=github&logoColor=2dd4bf" alt="GitHub">

## <img src="assets/icons/opensource.svg" width="20" height="20" alt=""> Open source

The tools I publish are open source, and I picked Godot for my game for the same reason. I want to build on something nobody can take away. I haven't contributed to other projects yet. That's next. With more and more code written by AI, I think open, readable software matters more, and I want to help keep it around.

## <img src="assets/icons/currently.svg" width="20" height="20" alt=""> Currently

<table>
  <tr><td><b>Reading</b></td><td><i>The Phoenix Project</i> &amp; <i>The Mythical Man-Month</i></td></tr>
  <tr><td><b>Building</b></td><td>The Claude Code mod catalog, EonHeart, the drawing app, Vivarium</td></tr>
  <tr><td><b>Learning</b></td><td>SpacetimeDB, Godot</td></tr>
</table>

## <img src="assets/icons/contact.svg" width="20" height="20" alt=""> Contact

<a href="https://www.linkedin.com/in/baeumli/"><img width="150" src="https://img.shields.io/badge/LinkedIn-1a1816?style=flat-square&logo=data:image%2Fsvg%2Bxml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHZpZXdCb3g9IjAgMCAyNCAyNCI%2BPHJlY3QgeD0iMi41IiB5PSIyLjUiIHdpZHRoPSIxOSIgaGVpZ2h0PSIxOSIgcng9IjMiIGZpbGw9Im5vbmUiIHN0cm9rZT0iIzJkZDRiZiIgc3Ryb2tlLXdpZHRoPSIyIiBzdHJva2UtbGluZWNhcD0icm91bmQiIHN0cm9rZS1saW5lam9pbj0icm91bmQiLz48Y2lyY2xlIGN4PSI4IiBjeT0iNy42IiByPSIxLjMiIGZpbGw9IiMyZGQ0YmYiLz48cGF0aCBkPSJNOCAxMXY2LjVNMTIgMTcuNVYxMU0xMiAxMy42YTIuOCAyLjggMCAwIDEgNS42IDB2My45IiBmaWxsPSJub25lIiBzdHJva2U9IiMyZGQ0YmYiIHN0cm9rZS13aWR0aD0iMiIgc3Ryb2tlLWxpbmVjYXA9InJvdW5kIiBzdHJva2UtbGluZWpvaW49InJvdW5kIi8%2BPC9zdmc%2B" alt="LinkedIn"></a>
<a href="https://discord.com/users/453479902575067136"><img width="238" src="https://img.shields.io/badge/Discord_%C2%B7_.lunyx.-1a1816?style=flat-square&logo=discord&logoColor=2dd4bf" alt="Discord: .lunyx."></a>
<img width="354" src="https://img.shields.io/badge/baeumli.dev_%C2%B7_coming_soon-1a1816?style=flat-square&logo=data:image%2Fsvg%2Bxml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHZpZXdCb3g9IjAgMCAyNCAyNCI%2BPGNpcmNsZSBjeD0iMTIiIGN5PSIxMiIgcj0iOSIgZmlsbD0ibm9uZSIgc3Ryb2tlPSIjMmRkNGJmIiBzdHJva2Utd2lkdGg9IjIiIHN0cm9rZS1saW5lY2FwPSJyb3VuZCIgc3Ryb2tlLWxpbmVqb2luPSJyb3VuZCIvPjxwYXRoIGQ9Ik0zIDEyaDE4TTEyIDNjMi42IDIuNiAzLjggNS42IDMuOCA5cy0xLjIgNi40LTMuOCA5Yy0yLjYtMi42LTMuOC01LjYtMy44LTlzMS4yLTYuNCAzLjgtOVoiIGZpbGw9Im5vbmUiIHN0cm9rZT0iIzJkZDRiZiIgc3Ryb2tlLXdpZHRoPSIyIiBzdHJva2UtbGluZWNhcD0icm91bmQiIHN0cm9rZS1saW5lam9pbj0icm91bmQiLz48L3N2Zz4%3D" alt="Website baeumli.dev, coming soon">

Based in Zurich. I answer in German or English.
