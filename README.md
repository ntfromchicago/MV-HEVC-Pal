# MV-HEVC Pal

<img width="752" alt="version 1 0 screen shot" src="https://github.com/user-attachments/assets/062e0cff-5e2d-4b71-8c72-fcf8692c7306" />

THIS IS A BETA BUILT WITH Xcode 26 beta + tested on macOS 26 beta. You have been warned.

It says it runs on Intel but the commands it uses do not. Sorry to everyone with an older Mac.

To download the .zip containing the app, look at the Releases and download the latest version.

## Summary

MV-HEVC Pal is a utility that converts 3D video files into MV-HEVC for use on Apple Vision Pro.

Special thanks and full credit goes to Mike Swanson for the [spatial video tools](https://blog.mikeswanson.com/spatial-video/) that MUST be installed for MV-HEVC Pal to work.

Special thanks to Andrew Hazelden for [Spatial Metadata GUI](https://github.com/Kartaverse/Spatial-Metadata), which greatly influenced this app.

Have feedback? Report an issue or email me at uxuios@gmail.com, and I'll investigate.

## Key Features

One of the cool things about building utilities like this in SwiftUI is the stuff you get out of the box. For example, the ability to open multiple encoding sessions at once. (I found this by accident. I don't know if it works, but I kept it in so others can be the guinea pig.)

But otherwise, it pretty much does what it says: Convert videos into MV-HEVC format.

All encoding is done locally. MV-HEVC Pal has no analytics, usage tracking or internet dependencies. Your data privacy is safe with MV-HEVC Pal, but obviously this is the internet, so trust but verify with [Charles](https://www.charlesproxy.com) or similar tools. Other than Mike Swanson's spatial, MV-HEVC Pal does not use third-party frameworks.

## Requirements

✅ An Apple Silicon Mac running macOS 26 beta (it may work on older macOS versions but I haven't tested)

I'm pretty sure Apple Silicon is required, even though this app may still open on Intel Macs.

✅ The CLI package [spatial](https://blog.mikeswanson.com/spatial-video/) by Mike Swanson. The easiest way is via [Homebrew](https://brew.sh/).
		
	# Once Homebrew is installed, run this command in the macOS Terminal app:
	brew install spatial
		
	# spatial should automatically install to:
	/opt/homebrew/bin/spatial

	# To uninstall, run this command in Terminal:
	brew uninstall spatial

The spatial tools must be installed at `/opt/homebrew/bin/spatial` (which should happen automatically if you use Homebrew) for MV-HEVC Pal to work. You'll get a warning if the app can't find these tools when you try to encode.

## Why This Exists

I wrote this app because Spatial Metadata GUI uses Xojo for its UI. Nothing wrong with Xojo, but the release of Liquid Glass sparked my interest in building this purely in SwiftUI.

In addition, I am writing a book on Designing With SwiftUI + AI so I used a lot of the techniques in the book on this project. This app is proof the book worked! (Those who buy the book will get a copy of the source code, which I have not yet open sourced.)

If you're running macOS 26, download the .zip file to try it out. It uses Icon Composer for the icon and there are other little touches of Liquid Glass in action. 

It also fixes some of the UI issues I wanted to tweak and make it feel a little more native, such as:

🛠️ A proper progress bar to track encoding progress

🛠️ Replacing the bitrate setting with quality setting

🛠️ Disables encode settings while encoding

🛠️ Help text to explain encode options

🛠️ Improved messaging and cleaner layout that's ready for macOS 26

I'll be tuning the source code until macOS goes live in production.

## Version History

THIS IS A BETA BUILT WITH Xcode 26 beta + tested on macOS 26 beta. You have been warned.

### Version 1.0 (2025-06-24)

- Initial release

