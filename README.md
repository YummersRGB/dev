# Wii Dev

This repository contains a complete multi-file C project for a custom Nintendo Wii homebrew game, along with a modern, responsive web page for distributing the download. 

## Project Structure

* `/dev/` - The compiled application folder ready for an SD card (contains `meta.xml` and the built `boot.dol`).
* `/src/` - The C source code and headers for the game.
* `/web/` - HTML and CSS files for the download portal.
* `Makefile` - Build instructions for the devkitPPC toolchain.

## Prerequisites

To compile the Wii executable from the source code, you need to install the official homebrew toolchain:
1. Install [devkitPro](https://devkitpro.org/wiki/Getting_Started).
2. Ensure you install the **devkitPPC** toolchain and **libogc** libraries via the devkitPro pacman package manager.
3. Make sure your environment variables (like `DEVKITPPC` and `DEVKITPRO`) are properly configured.

## Compilation

1. Open your terminal or command prompt.
2. Navigate to the root directory of this project (where the `Makefile` is located).
3. Run the compile command:
   ```bash
   make
