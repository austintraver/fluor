# Fluor

[![Swift](https://img.shields.io/badge/Swift-4.0-orange.svg?style=flat)](https://developer.apple.com/swift/)
![version](https://img.shields.io/badge/macOS-10.11+-green.svg?style=flat)
[![License](https://img.shields.io/badge/license-MIT-71787A.svg)](https://tldrlegal.com/license/mit-license)

# About

**Fluor** is a tool that allows you to automatically change the behavior of the keyboard's fn keys depending on the active application. It's that simple.

# Installation

There's two main ways to install **Fluor**:

## Option 1 – Package Manager

* Install via [Homebrew Cask](https://caskroom.github.io):

    ```shell
    brew install --cask fluor
    ```

## Option 2 – Manual Installation

* Download the [latest release](https://github.com/Pyroh/Fluor/releases), open the `.dmg` file, and drag the application to your `/Applications` folder.

You can also build it from source, but this is not recommended if your are only going to use **Fluor** in the regular way, and not hack it.

# How does it work?

**Fluor** lies in your status bar and makes you see instantaneously which mode your keyboard is on:

<img src="resources/statusbar.png" width=327pt>

* <img src="Fluor/Assets.xcassets/IconAppleMode.imageset/iconAppleMode@2x.png" width=16pt>

    * This means that the keyboard's `Fn` key behaves like the special Apple function keys (Volume, Play/Pause, Skip, etc).

* <img src="Fluor/Assets.xcassets/iconOtherMode.imageset/iconOtherMode@2x.png" width=16pt>

    * This means that the keyboard's fn keys act like these good old function keys (F1, F2, F3, you got it...).

## Fluor's Menu

This is what you get when you click on **Fluor** in the status bar:

<img src="resources/mainmenu.png" width=279pt>

You can choose the default mode. Whenever **Fluor** runs it will activate the default mode for your keyboard's fn keys.

**Fluor** also displays the active application and its associated rule that you can change on the go.

<img src="Fluor/Assets.xcassets/DefaultMode.imageset/DefaultModeLight@2x.png" width=16pt> is the default rule and means that the application will adopt default Fluor's keyboard behaviour.

You can also disable **Fluor** if you need to. It will set the keyboard's behaviour as it was prior to the application's launch.

## Rules Editor

<img src="resources/ruleseditor.png" width=412pt>

This panel allows you to see all the rules you set at once. You can modify or delete any rule. Adding a rule will prompt a file selector in which you'll be able to select the application you want to set a rule for.

## Running Applications

<img src="resources/runningapps.png" width=412pt>

Sometimes it is not possible to select an application in the *Rules Editor*, especially for Steam games. This panel lets you set a rule for any running application. Of course the rules you set in this panel will be available directly in the *Rules Editor*. You can also remove a rule by setting the application behaviour to <img src="Fluor/Assets.xcassets/DefaultMode.imageset/DefaultModeLight@2x.png" width=16pt>, it will also disappear from the *Rules Editor* panel.

# Why is it open source ?

I made **Fluor** because I needed such an application. I wanted it simple, nicely designed and free and I didn't find such a thing on the internet. Once it was done I used it for a little while, cleaned up the code and decided to give it to others for free. What was a requirement for me can well be a requirement for others too.
You'd argue that such a non-sandboxed app had no chance to hit the AppStore and you'd be right. But if I had the chance it would have remained free and open-source. I don't think there's many people needing such an app and I prefer seeing it used by a wider range of people.

This app is also built using open-source code, that's why I think it belongs to this world. And if someone learns something looking at the code I'll be happy 😃.

# Contributing

All contributions are welcome. Fork it, hack it and make a pull request.

# License

**Fluor** is released under the MIT license. See LICENSE for details.

Some of [**fntoggle**](https://github.com/nelsonjchen/fntoggle)'s code was used. As its author [wrote](https://github.com/nelsonjchen/fntoggle#license) it could be released under the GPL2 license.

The code also uses [**LaunchAtLoginController**](https://github.com/Mozketo/LaunchAtLoginController) which is Copyright (c) 2010 Ben Clark-Robinson, ben.clarkrobinson@gmail.com and is released under the MIT LICENSE.
