# Liquid-Pull-To-Refresh

A customizable pull-to-refresh widget for Flutter projects, featuring an attractive liquid physics-based animation.

![Demo Gif](display/demo.gif)

## Table of Contents

1. [Project Overview](#project-overview)
2. [Installation Instructions](#installation-instructions)
3. [Usage Guide](#usage-guide)
4. [Features and Functionality](#features-and-functionality)
5. [Contributing Guidelines](#contributing-guidelines)
6. [License Information](#license-information)
7. [Contact Information](#contact-information)

## Project Overview

Liquid-Pull-To-Refresh is a Flutter widget that provides an attractive and customizable pull-to-refresh experience for your projects. It leverages Flutter's built-in animation capabilities and uses the liquid physics engine provided by the Flutter Physics package to create a visually engaging liquid effect during the refresh process.

### Technologies and Tools

The project is built using:

- **Flutter:** The popular open-source UI software development kit that helps in building natively compiled applications for mobile, web, and desktop from a single codebase.
- **Flutter Physics:** A package providing common physics algorithms and related utilities for use in Flutter applications.

These technologies are crucial to the project as they contribute to its cross-platform compatibility, performance, and the liquid physics-based animation effect.

## Installation Instructions

To use Liquid-Pull-To-Refresh in your project, follow these steps:

1. Add the following dependency to your `pubspec.yaml` file:

```yaml
dependencies:
  liquid_pull_to_refresh: ^1.0.0
```

2. Run the following command to install the package:

```bash
$ flutter pub get
```

3. Finally, import the package in your Dart code:

```dart
import 'package:liquid_pull_to_refresh/liquid_pull_to_refresh.dart';
```

## Usage Guide

To use Liquid-Pull-To-Refresh, simply wrap your ListView, GridView, or any other scrollable widget with the `LiquidPullToRefresh` widget:

```dart
LiquidPullToRefresh(
  onRefresh: _handleRefresh,
  child: ListView.builder(
    itemBuilder: (context, index) => ListTile(title: Text('Item $index')),
    itemCount: 30,
  ),
);
```

In this example, `_handleRefresh` is a callback function that will be invoked when the user triggers a refresh. This function should return a `Future` to indicate the completion of the refresh process.

## Features and Functionality

- Attractive liquid physics-based animation during the refresh process.
- Customizable colors, opacity, and other appearance attributes.
- Adjustable refresh trigger threshold and other behavior settings.
- Compatible with both Android and iOS platforms.

## Contributing Guidelines

To contribute to this project, please refer to the [CONTRIBUTING.md](CONTRIBUTING.md) file for detailed guidelines.

## License Information

This project is licensed under the [MIT License](LICENSE). For more information, please refer to the [LICENSE](LICENSE) file.

## Contact Information

For any questions, feedback, or issues, please feel free to reach out to the repository owner or create an issue in the GitHub repository. Your input and support are greatly appreciated.

Owner: [Youssef](https://github.com/thisisyoussef)
Repository: [Liquid-Pull-To-Refresh](https://github.com/thisisyoussef/Liquid-Pull-To-Refresh)