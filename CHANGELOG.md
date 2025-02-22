# Change Log

## Dangerzone 0.4.0

- Platform support: Re-add Fedora 37 support
- Platform support: Add Debian Bookworm (12) support ([issue #172](https://github.com/freedomofpress/dangerzone/issues/172))
- Platform support: Reinstate Ubuntu Focal support ([issue #206](https://github.com/freedomofpress/dangerzone/issues/206))
- Platform support: Add Ubuntu 22.10 "Kinetic Kudu" support ([issue #265](https://github.com/freedomofpress/dangerzone/issues/265))
- Feature: Support bulk conversion to safe PDFs ([issue #77](https://github.com/freedomofpress/dangerzone/issues/77))
- Feature: Option to archive unsafe directories ([issue #255](https://github.com/freedomofpress/dangerzone/pull/255))
- Feature: Support python 3.10
- Feature: When quitting while still converting, confirm if user is sure
- Bug fix: Fix unit tests on Windows
- Bug fix: Do not hardcode "docker" in help messages, now that Podman is also used ([issue #122](https://github.com/freedomofpress/dangerzone/issues/122))
- Bug fix: Failed execution no longer produces an empty "safe" documents ([issue #214](https://github.com/freedomofpress/dangerzone/issues/214))
- Bug fix: Malfunctioning "New window" logic was replaced with multi-doc support ([issue #204](https://github.com/freedomofpress/dangerzone/issues/204))
- Bug fix: re-adds support for 'open with Dangerzone' from finder on macOS ([issue #268](https://github.com/freedomofpress/dangerzone/issues/268))
- Bug fix: (macOS) quit Dangerzone when main window is closed ([issue #271](https://github.com/freedomofpress/dangerzone/issues/271))


## Dangerzone 0.3.2
- Bug fix: some non-ascii characters like “ would prevent Dangerzone from working  ([issue #144](https://github.com/freedomofpress/dangerzone/issues/144))
- Bug fix: error where Dangerzone would show "permission denied: '/tmp/input_file'" ([issue #157](https://github.com/freedomofpress/dangerzone/issues/157))
- Bug fix: remove containers after use, enabling Dangerzone to run after 1000+ converted docs ([issue #197](https://github.com/freedomofpress/dangerzone/pull/197))
- Security: limit container capabilities, run in container as non-root and limit privilege escalation ([issue #169](https://github.com/freedomofpress/dangerzone/issues/169))


## Dangerzone 0.3.1

- Bug fix: Allow converting documents on different mounted filesystems than the container volume
- Bug fix: In GUI mode, don't always OCR document
- Bug fix: In macOS, fix "open with" Dangerzone so documents are automatically selected
- Windows: Change packaging to avoid anti-virus false positives

## Dangerzone 0.3

- Removes the need for internet access by shipping the Dangerzone container image directly with the software
- Friendly user experience with a progress bar
- Support for Macs with M1 chips

## Dangerzone 0.2.1

- Switch from Docker to Podman for Linux
- Improve CLI colors

## Dangerzone 0.2

- Command line support and improved terminal output
- Additional container hardening
- Fix macOS crash on quit
- Fix --custom-container CLI argument

## Dangerzone 0.1.5

- Add support for macOS Big Sur
- Drop support for Ubuntu 19.10

## Dangerzone 0.1.4

- Suppress confusing stderr output, and fix bug when converting specific documents
- Switch from PyQt5 to PySide2
- Improve Windows and Mac packaging
- Add support for Fedora 32

## Dangerzone 0.1.3

- Add support for Ubuntu 20.04 LTS (#79)
- Prevent crash in macOS if specific PDF viewers are installed (#75)

## Dangerzone 0.1.2 (Linux only)

- Add support for Ubuntu 18.04 LTS

## Dangerzone 0.1.1

- Fix macOS bug that caused a crash on versions earlier than Catalina
- Fix macOS app bundle ODF extensions (`.ods .odt`)
- Allow Linux users to type their password instead of adding their user to the `docker` group
- Use Docker instead of Podman in Fedora
- Allow the use of either OS-packaged Docker or Docker CE in Linux
- Allow opening `.docm` files
- Allow using a custom container for testing

## Dangerzone 0.1

- First release
