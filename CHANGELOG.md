# CHANGELOG

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog],
and this project adheres to [Semantic Versioning].

<!-- markdownlint-disable MD024 -->

## Unreleased

## [0.7.1] - 2024-07-02

### Changed

- Logo has changed.
- Apply the template version 0.7.0

## [0.7.0] - 2024-06-26

### Changed

- Rename the package from COPIERTemplate.jl to BestieTemplate.jl

## [0.6.1] - 2024-06-21

### Changed

- Small improvements to templates

## [0.6.0] - 2024-06-14

### Changed

- Rename files in docs/src/ 90-developer to 91 and 90-reference to 95 (#273)

## [0.5.4] - 2024-06-11

### Changed

- Indentation is now a required question

## [0.5.3] - 2024-06-10

### Changed

- Update documentation in various places
- Add developer documentation for dealing with the template

### Fixed

- Template had bad double quotes instead of single in the Test.yml workflow

## [0.5.2] - 2024-06-08

### Added

- Update function that calls copier's run_update (#113)
- Safeguard to avoid running generate when you want update (#247)

### Changed

- Improve skip section in README.md and make small corrections in the template

## [0.5.1] - 2024-06-07

### Added

- New question: AddPrecommit to add pre-commit related files (#231)
- New question: AddGitHubTemplates to add issue and PR templates (#233)
- New question: AnswerStrategy to choose between using recommended, minimum, or ask every question (#235)
- New question: AddCopierCI to add Copier.yml (#237)

### Changed

- Issue checklists are now just text (#234)

## [0.5.0] - 2024-06-06

### Added

- New question: SimplifiedPRTest to simplify the testing on Pull Requests (#105)
- New question: AddAllcontributors to add a section and config for <https://allcontributors.org> (#26)
- `copy`, `recopy` and `update` from the copier API (#142)
- When applying to existing projects, read Project.toml to infer a few values (#116)
- Automatically determines the `PackageName` from the destination folder (#151)

### Changed

- Adds `data` positional argument to `generate` (#142)
- An internal module `Copier` was created with the wrapper functions
- Use lychee for link-checker instead of markdown-link-checker (#160)

### Removed

- The `generate_missing_uuid` argument was removed, since it can be generated via Jinja (#189)

## [0.4.0] - 2024-05-31

### Added

- Pre-commit update workflow (#91)

### Changed

- Signature of generate now accepts source path, which defaults to the URL (#174)

## [0.3.2] - 2024-05-30

### Added

- More reader-friendly README (#144)
- Add author names to licenses (#145)
- Consistent caching in GitHub workflows (#53)

## [0.3.1] - 2024-05-23

### Added

- Dependabot (#52)

## [0.3.0] - 2024-05-17

### Added

- Indentation option (#44)
- CODE_OF_CONDUCT (#25)
- Issue and Pull Request templates (#33)
- AskAdvancedQuestions question to allow stopping early (#67)

### Changed

- Update Cirrus CI image_family (#31)
- Prefix some doc files with a number and generate the pages programmatically (#32)
- Reestructure and improve the documentation (#77)

### Fixed

- Coverage now checks main branch (#65)

## [0.2.5] - 2024-02-23

### Fixed

- nightly key was duplicated (#49)

## [0.2.4] - 2023-12-21

### Fixed

- pipx link changed

## [0.2.3] - 2023-10-31

### Changed

- Add `workflow_dispatch` to Test.yml

### Fixed

- Windows support

## [0.2.2] - 2023-10-02

### Fixed

- Don't skip contributing.md and developer.md on updates

## [0.2.1] - 2023-10-02

### Added

- asciinema link in the README

### Fixed

- Text and typos on contribuing and developer

## [0.2.0] - 2023-09-24

### Changed

- First Julia release

## [0.1.9] - 2023-09-24

### Fixed

- Remove `_exclude` section from `copier.yml`

## [0.1.8] - 2023-09-24

### Added

- Should be installable as a Julia package now
- Use PythonCall to run copier directly from the Julia package

### Changed

- Move template to subdirectory

### Fixed

- Allow failure in nightly Julia Test.yml workflow

## [0.1.7] - 2023-09-22

### Changed

- Rename Compliance to Copier in various places (including this CHANGELOG)

## [0.1.6] - 2023-09-22

### Added

- Use pre-commit to prevent adding .rej files and ongoing merge conflicts
- Add configuration file for markdown link checker and ignore @ref

### Changed

- Only ignore Project.toml, not all toml
- Change markdown-lint to fix version

## [0.1.5] - 2023-09-22

### Fixed

- Properly fix copier update when there are conflicts

## [0.1.4] - 2023-09-22

### Fixed

- Fix copier update when there are conflicts

## [0.1.3] - 2023-09-21

### Added

- Run pre-commit in the Copier workflow to commit the formatters change as well

### Changed

- Add a basic structure for the copy's CITATION.cff

## [0.1.2] - 2023-09-16

### Added

- Zenodo DOI
- Instruction to add a Zenodo DOI
- Badge on README

### Changed

- Documenter compat is 1
- Remove keywords strict and linkcheck from docs/make.jl

### Fixed

- File docs/make.jl should not be skipped

## [0.1.1] - 2023-09-15

### Added

- Add CITATION.cff

### Fixed

- Exclude docs/assets/logo.png

## [0.1.0] - 2023-09-12

- Initial release

<!-- Links -->

[keep a changelog]: https://keepachangelog.com/en/1.0.0/
[semantic versioning]: https://semver.org/spec/v2.0.0.html

<!-- Versions -->

[0.7.1]: https://github.com/abelsiqueira/BestieTemplate.jl/releases/tag/v0.7.1
[0.7.0]: https://github.com/abelsiqueira/BestieTemplate.jl/releases/tag/v0.7.0
[0.6.1]: https://github.com/abelsiqueira/BestieTemplate.jl/releases/tag/v0.6.1
[0.6.0]: https://github.com/abelsiqueira/BestieTemplate.jl/releases/tag/v0.6.0
[0.5.4]: https://github.com/abelsiqueira/BestieTemplate.jl/releases/tag/v0.5.4
[0.5.3]: https://github.com/abelsiqueira/BestieTemplate.jl/releases/tag/v0.5.3
[0.5.2]: https://github.com/abelsiqueira/BestieTemplate.jl/releases/tag/v0.5.2
[0.5.1]: https://github.com/abelsiqueira/BestieTemplate.jl/releases/tag/v0.5.1
[0.5.0]: https://github.com/abelsiqueira/BestieTemplate.jl/releases/tag/v0.5.0
[0.4.0]: https://github.com/abelsiqueira/BestieTemplate.jl/releases/tag/v0.4.0
[0.3.2]: https://github.com/abelsiqueira/BestieTemplate.jl/releases/tag/v0.3.2
[0.3.1]: https://github.com/abelsiqueira/BestieTemplate.jl/releases/tag/v0.3.1
[0.3.0]: https://github.com/abelsiqueira/BestieTemplate.jl/releases/tag/v0.3.0
[0.2.5]: https://github.com/abelsiqueira/BestieTemplate.jl/releases/tag/v0.2.5
[0.2.4]: https://github.com/abelsiqueira/BestieTemplate.jl/releases/tag/v0.2.4
[0.2.3]: https://github.com/abelsiqueira/BestieTemplate.jl/releases/tag/v0.2.3
[0.2.2]: https://github.com/abelsiqueira/BestieTemplate.jl/releases/tag/v0.2.2
[0.2.1]: https://github.com/abelsiqueira/BestieTemplate.jl/releases/tag/v0.2.1
[0.2.0]: https://github.com/abelsiqueira/BestieTemplate.jl/releases/tag/v0.2.0
[0.1.9]: https://github.com/abelsiqueira/BestieTemplate.jl/releases/tag/v0.1.9
[0.1.8]: https://github.com/abelsiqueira/BestieTemplate.jl/releases/tag/v0.1.8
[0.1.7]: https://github.com/abelsiqueira/BestieTemplate.jl/releases/tag/v0.1.7
[0.1.6]: https://github.com/abelsiqueira/BestieTemplate.jl/releases/tag/v0.1.6
[0.1.5]: https://github.com/abelsiqueira/BestieTemplate.jl/releases/tag/v0.1.5
[0.1.4]: https://github.com/abelsiqueira/BestieTemplate.jl/releases/tag/v0.1.4
[0.1.3]: https://github.com/abelsiqueira/BestieTemplate.jl/releases/tag/v0.1.3
[0.1.2]: https://github.com/abelsiqueira/BestieTemplate.jl/releases/tag/v0.1.2
[0.1.1]: https://github.com/abelsiqueira/BestieTemplate.jl/releases/tag/v0.1.1
[0.1.0]: https://github.com/abelsiqueira/BestieTemplate.jl/releases/tag/v0.1.0
