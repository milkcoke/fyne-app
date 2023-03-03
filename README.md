
# Introduction
Toolbox provides you developer tool installer kit as latest version. \
This is beta version application.

## Demo
![toolbox_demo](https://user-images.githubusercontent.com/48945177/222765964-7db981e6-f862-46be-8033-f3ba3b12169a.gif)

## Quick start
First build time is long since internally transfile from C/C++ to go.

```bash
# download this repository and execute
$ go run .
```

### Prerequisite
- [GNU make](https://gnuwin32.sourceforge.net/packages/make.htm)
- [Go](https://go.dev/dl/)
- [Fyne](https://developer.fyne.io/started/) 
- msys2 \
C compiler for windows

Enable Go Modules integration in IntelliJ IDEA.

## What's the Fyne?
Fyne uses single binding to compile our app with existing graphics driver independent on Operation System.



### Packaging
#### 1. Install fyne cmd
```bash
$ go install fyne.io/fyne/v2/cmd/fyne@latest
```

#### 2. Prepare icon of app

#### 3. Input cli
Refer to [this docs](https://developer.fyne.io/started/packaging)
```bash
# change directory including main.go
$ cd [PATH]
$ fyne package --appVersion [version] -name [app-name] -icon [app-icon-path] -release
```

> This is just only usable on your machine. \
> This binary files generated by cli doesn't work any other OS.

### Register application
You need give some money about $100 / year to Apple or Microsoft for supporting cross-platform \
for signing your application assuring your app is secure.

## Test
I defined `Makefile` for integration testing.
```bash
# You can execute all test codes in this project.
$ make test
```
