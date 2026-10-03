# Changelog

All notable changes to this project are documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.1.0/), and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [Unreleased]

## [1.6.0] - 2026-10-02

### Added

- **Website Ignore List** setting. Links containing any of the listed strings (comma or newline separated) are not processed by the plugin at all: they are pasted or dropped as-is, and the "Enhance existing URL" command leaves them untouched. Unlike the Website Blacklist, which still converts matching links to markdown links titled with the domain, ignored links are never converted.
- A notice is shown when a title can't be fetched because there is no internet connection.
- Instructions in the README for installing this fork with BRAT.

## [1.5.5] - 2024-12-04

See the [upstream release notes](https://github.com/zolrath/obsidian-auto-link-title/releases/tag/1.5.5) for this and earlier versions.

[Unreleased]: https://github.com/coreyx/obsidian-auto-link-title/compare/1.6.0...HEAD
[1.6.0]: https://github.com/zolrath/obsidian-auto-link-title/compare/1.5.5...coreyx:obsidian-auto-link-title:1.6.0
[1.5.5]: https://github.com/zolrath/obsidian-auto-link-title/releases/tag/1.5.5
