# obs-cli

[![GoDoc](https://godoc.org/github.com/golang/gddo?status.svg)](https://godoc.org/github.com/muesli/obs-cli)
[![Go ReportCard](http://goreportcard.com/badge/muesli/obs-cli)](http://goreportcard.com/report/muesli/obs-cli)

OBS-cli is a command-line remote control for OBS. It requires the
[obs-websocket](https://github.com/Palakis/obs-websocket) plugin to be installed on your system.

## Installation

### Packages & Binaries

On Arch Linux you can simply install the package from the AUR:

    yay -S obs-cli

Or download a binary from the [releases](https://github.com/muesli/obs-cli/releases)
page. Linux (including ARM) binaries are available, as well as Debian and RPM
packages.

### Build From Source

Alternatively you can also build `obs-cli` from source. Make sure you have a
working Go environment (Go 1.11 or higher is required). See the
[install instructions](http://golang.org/doc/install.html).

To install obs-cli, simply run:

    go get github.com/muesli/obs-cli

## Usage

Start streaming:

```bash
obs-cli start-stream
```

Stop streaming:

```bash
obs-cli stop-stream
```

Start recording:

```bash
obs-cli start-recording
```

Stop recording:

```bash
obs-cli stop-recording
```

Toggle recording:

```bash
obs-cli toggle-recording
```

Switch to a scene:

```bash
obs-cli switch-scene <scene>
```

Change a FreeType text label:

```bash
obs-cli change-text <label> <text>
```

List all items of a scene:

```bash
obs-cli list-sceneitems <scene>
```

Make a scene-item visible:

```bash
obs-cli show-sceneitem <scene> <item>
```

Hide a scene-item:

```bash
obs-cli hide-sceneitem <scene> <item>
```

List special sources:

```bash
obs-cli list-sources
```

Toggle mute status of a source:

```bash
obs-cli toggle-mute <source>
```
