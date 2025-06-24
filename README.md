# MV-HEVC Pal

<img width="752" alt="version 1 0 screen shot" src="https://github.com/user-attachments/assets/062e0cff-5e2d-4b71-8c72-fcf8692c7306" />

THIS IS A BETA BUILT WITH Xcode 26 beta + tested on macOS 26 beta. You have been warned.

It says it runs on Intel but the commands it uses do not. Sorry to everyone with an older Mac.

## Summary

MV-HEVC Pal is a utility that takes SBS 3D videos and converts them into MV-HEVC files for use on Apple Vision Pro.

Special thanks and full credit goes to Mike Swanson for the spatial video tools that must be installed for MV-HEVC Pal to work.

Special thanks to Andrew Hazelden for Spatial Metadata GUI, which I have used for work, and which greatly influenced this app.

Have feedback? Feel free to report an issue or email me at uxuios@gmail.com and I'll investigate.

## Key Features

One of the cool things about building utilities like this in SwiftUI is the stuff you get out of the box. For example, the ability to open multiple encoding sessions at once. (I found this by accident. I don't know if it works, but I kept it in so others can be the guinea pig.)

But otherwise, it pretty much does what it says: Convert 3D flat videos into MV-HEVC, with the same adjustments available as in similar apps.

All encoding is done locally, and there are no analytics, usage tracking or bug reporting in this app. Your data privacy is safe with MV-HEVC Pal, but obviously this is the internet, so trust but verify with Postman or whatever packet sniffer you want to use while running this. Other than spatial, it does not use any third-party frameworks.

## Requirements

An Apple Silicon Mac running macOS 26 beta

It may work on older macOS versions but I haven't tested.

I'm pretty sure Apple Silicon is required, even though this app may still open on Intel Macs.

You also need to install [spatial](https://blog.mikeswanson.com/spatial-video/) by Mike Swanson, as a command-line interface. The easiest way is via [Homebrew(https://brew.sh/).
		
		# Once Homebrew is installed, run this command in the macOS Terminal app:
		brew install spatial
		
		# The Spatial CLI app now lives on your hard disk at:
		/opt/homebrew/bin/spatial

		# To uninstall, run the uninstall command in Terminal:
		brew uninstall spatial

The spatial tools must be installed at /opt/homebrew/bin/spatial (which should happen automatically) for MV-HEVC Pal to work. You'll get a warning if the app can't find these tools when you try to encode.


## Why This Exists

I wrote this app because Spatial Metadata GUI uses Xojo for its UI. Nothing wrong with Xojo, but the release of Liquid Glass sparked my interest in seeing if I could build this purely as a SwiftUI app.

In addition, I am writing a book on Designing With SwiftUI + AI so I used a lot of the techniques in the book on this project. This app is proof the book worked! (Those who buy the book with get a copy of the source code, which I have not yet open sourced.)

If you're running macOS 26, download the .zip file to try it out. It uses Icon Composer for the icon and there are other little touches of Liquid Glass in action. It also fixes some of the little UI things that I wanted to tweak and make it feel a little more native.

I'll be tuning the source code until macOS goes live in production.

## Version History

THIS IS A BETA BUILT WITH Xcode 26 beta + tested on macOS 26 beta. You have been warned.

### Version 1.0 (2025-06-24)

- Initial release

