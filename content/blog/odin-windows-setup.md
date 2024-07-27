+++
title = 'Getting started with Odin on Windows'
date = 2024-07-16T20:13:27+02:00
draft = false
tags = [
  "odin",
  "programming",
]
+++

## Introduction

I am currently making a game using Odin. It is developed on Linux, but
cross-compilation is not supported yet, so I have to use Windows, whether I
like it or not.

Unfortunately, installation on Windows is quite different from Linux, and
tutorials about it aren't specific about the exact tools to install.

Note that I am on Windows 10, and I won't compile from source.

## Installing Visual Studio

First, download the Visual Studio [installer], preferably the latest Community
version.

Start the installer, and when it asks you to choose the components to install,
scroll and select *Desktop development in C++*.

Keep only the first option (C++ compiler) and Windows 10 (or 11, depending on
your Windows version) SDK. Choose the latest, it doesn't matter if versions
don't match exactly.

## Using Odin

You can download the latest release [here]. Extract the zip to a specific folder
(for instance, *C:\Odin*).

### Checking if it works

Create the following program and save it as the file *main.odin* :

```odin
package main

import "core:fmt"

main :: proc() {
  fmt.println("Hellope!")
}
```

Now to run it, you have to open "x64 Native Tools Command Prompt for
VS2022" (type it on the Windows search bar), then go to the folder path in
which your Odin file is.

To do so, type `cd path\to\main.odin` (naturally, replace *path\to* by the path of your odin file).

Then `path\to\odin run main.odin`.

For example, if your Odin executable is in the folder *C:\Odin*, then you will write :

`C:\Odin\odin run main.odin`

### Add Odin compiler to the path

It works, but it is annoying to type *C:\Odin\odin* every time I want to
call the compiler. Wouldn't it be better if you could simply use `odin` instead ?

Here are the instructions to do so.

On Windows search bar, type *environment variable* and choose the first option
that appears. Click on the corresponding button on the bottom right.

Then, on the *System variables* section, look for one called *Path*, and
double-click on it. Press *New* and write the path to the folder containing the
executable.

Open a new command prompt (if you got one opened before adding to the path, it
won't work) and type `odin`. If you don't get any error, congratulations!

[installer]: https://visualstudio.microsoft.com/downloads/
[here]: https://github.com/odin-lang/Odin/releases/latest
