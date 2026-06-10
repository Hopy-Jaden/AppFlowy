<h1 align="center" style="margin:0"> AppFlowy_Flutter</h1>
<div align="center">
  <img src="https://img.shields.io/badge/Flutter-v3.13.19-blue"/>
  <img src="https://img.shields.io/badge/Rust-v1.70-orange"/>
</div>

> Documentation for Contributors

This Repository contains the codebase for the frontend of the application, currently we use Flutter as our frontend framework.

### Platforms Supported Using Flutter 💻

- Linux
- macOS
- Windows
  > We are actively working on support for Android & iOS!

_Additionally, we are working on a Web version built with Tauri!_

### Am I Eligible to Contribute?

Yes! You are eligible to contribute, check out the ways in which you can [contribute to AppFlowy](https://docs.appflowy.io/docs/documentation/software-contributions/contributing-to-appflowy). Some of the ways in which you can contribute are:

- Non-Coding Contributions
  - Documentation
  - Feature Requests and Feedbacks
  - Report Bugs
  - Improve Translations
- Coding Contributions

To contribute to `AppFlowy_Flutter` codebase specifically (coding contribution) we suggest you to have basic knowledge of Flutter. In case you are new to Flutter, we suggest you learn the basics, and then contribute afterwards. To get started with Flutter read [here](https://flutter.dev/docs/get-started/codelab).

### What OS should I use for development?

We support all OS for Development i.e. Linux, MacOS and Windows. However, most of us promote macOS and Linux over Windows. We have detailed [docs](https://docs.appflowy.io/docs/documentation/appflowy/from-source/environment-setup) on how to setup `AppFlowy_Flutter` on your local system respectively per operating system.

### Getting Started ❇

We have detailed documentation on how to [get started](https://docs.appflowy.io/docs/documentation/software-contributions/contributing-to-appflowy) with the project, and make your first contribution. However, we do have some specific picks for you:

- [Code Architecture](https://appflowy.gitbook.io/docs/essential-documentation/contribute-to-appflowy/architecture/frontend/frontend/codemap)
- [Styleguide & Conventions](https://docs.appflowy.io/docs/documentation/software-contributions/conventions/naming-conventions)
- [Making Your First PR](https://docs.appflowy.io/docs/documentation/software-contributions/submitting-code/submitting-your-first-pull-request)
- [All AppFlowy Documentation](https://docs.appflowy.io/docs/documentation/appflowy) - Contribution guide, build and run, debugging, testing, localization, etc.

### Need Help?

- New to GitHub? Follow [these](https://docs.appflowy.io/docs/documentation/software-contributions/submitting-code/setting-up-your-repositories) steps to get started
- Stuck Somewhere? Join our [Discord](https://discord.gg/9Q2xaN37tV), we're there to help you!
- Find out more about the [community initiatives](https://docs.appflowy.io/docs/appflowy/community).


### How to Set-up In Windows
1. Visual Studio 2022 
In section "All Downloads" => "Tools for Visual Studio 2022" => "Build Tools for Visual Studio 2022".
Launch vs_BuildTools.exe to install.
Choose "Desktop Development with C++"

2. vcpkg
Add vcpkg installation folder to your PATH environment variable.

3. Flutter
Install flutter, make sure version as 3.27.4.
flutter config --enable-windows-desktop
flutter doctor

4. LLVM
Add LLVM to PATH environment variable

5. Rust
Install rust

6. OpenSSl
Add Openssl to PATH like G:\Compilation\OpenSSL\bin

7. Perl

8. Protoc
Install protoc for dart activation of protoc_plugin


1. Run Commands
rustup default 1.80.1
cargo install cargo-make --force --locked
cargo install --force duckscript_cli --locked
dart pub global activate protoc_plugin 21.1.2
dart pub global activate fvm
fvm install 3.27.4
fvm use 3.27.4

2. create settings.json in .vscode folder
{
  "dart.flutterSdkPath": ".fvm/versions/3.27.4",
  "search.exclude": {
    "**/.fvm": true
  },
  "watcher.exclude": {
    "**/.fvm": true
  }
}

3. fvm dart pub global activate protoc_plugin 21.1.2
