<h1 align="center">Jellyfin Refresh Sparse Episodes Plugin</h1>
<h3 align="center">For use in the <a href="https://jellyfin.media">Jellyfin Project</a></h3>

<p align="center">
<a href="https://github.com/clowncracker/jellyfin-plugin-refreshsparse/actions/workflows/build-dotnet.yml">
<img alt="GitHub Workflow Status" src="https://img.shields.io/github/actions/workflow/status/clowncracker/jellyfin-plugin-refreshsparse/build-dotnet.yml">
</a>
<a href="https://github.com/clowncracker/jellyfin-plugin-refreshsparse">
<img alt="GPLv3 License" src="https://img.shields.io/github/license/clowncracker/jellyfin-plugin-refreshsparse.svg"/>
</a>
<a href="https://github.com/clowncracker/jellyfin-plugin-refreshsparse/releases">
<img alt="Current Release" src="https://img.shields.io/github/release/clowncracker/jellyfin-plugin-refreshsparse.svg"/>
</a>
</p>

## About

This plugin adds a scheduled job to search for and update episodes that are missing certain metadata.

Metadata that are checked:

- Name
    - Is it a date? "January 1, 2022"
    - User supplied list of substrings
- Overview
- Primary Image
- Number of provider IDs

Refresh all metadata/images options.

Pretend option to try it out without updating metadata.

## Compatibility

This branch targets **Jellyfin 12.0** (.NET 10). For Jellyfin 10.11, use the 5.0.0.0 release.

## Installation

Add [this link][1] to "Repositories" in Jellyfin settings, then install "Refresh Sparse Items" from the Catalog.

[1]: https://raw.githubusercontent.com/clowncracker/jellyfin-plugin-refreshsparse/master/manifest.json

## Build

1. To build this plugin you will need [.NET 10.x](https://dotnet.microsoft.com/download/dotnet/10.0).
2. Build the plugin with the following command:
