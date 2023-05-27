# Liquid Pull To Refresh

[![GitHub license](https://img.shields.io/github/license/thisisyoussef/Lliquid-Pull-To-Refresh.svg)](https://github.com/thisisyoussef/Liquid-Pull-To-Refresh/blob/master/LICENSE)

Liquid Pull To Refresh is a highly customizable Flutter library that adds liquid-inspired Pull-To-Refresh functionality to your apps. It provides a unique and visually engaging way to update content and adds a touch of dynamism.

## Table of Contents

- [Installation](#installation)
- [Usage](#usage)
- [Features and Functionality](#features-and-functionality)
- [Contributing](#contributing)
- [License](#license)
- [Contact](#contact)

## Installation

To use the library in your Flutter project, follow the steps below:

1. Add `liquid_pull_to_refresh` to your `pubspec.yaml` dependencies:

```yaml
dependencies:
  liquid_pull_to_refresh: ^latest_version
```

2. Install the package via the command line by running:

```bash
$ flutter pub get
```

## Usage

To use the Liquid Pull To Refresh widget, follow the steps below:

1. Import the `liquid_pull_to_refresh.dart` file into your project:

```dart
import 'package:liquid_pull_to_refresh/liquid_pull_to_refresh.dart';
```

2. Wrap your `ListView`, `GridView`, `CustomScrollView`, or any other scrollable widget in the `LiquidPullToRefresh`:

```dart
LiquidPullToRefresh(
  key: _refreshIndicatorKey,
  onRefresh: _handleRefresh,
  child: ListView.builder(
    itemBuilder: (context, index) => ListTile(title: Text("Item $index")),
    itemCount: 10,
  )
);
```

3. Create a function that performs the desired action on refresh (e.g., data fetching):

```dart
Future<void> _handleRefresh() async {
  // update data and state here
  await Future.delayed(Duration(seconds: 3));
}
```

For more information and advanced usage, please refer to the [example project](https://github.com/thisisyoussef/Liquid-Pull-To-Refresh/tree/master/example).

## Features and Functionality

- Unique and visually engaging liquid-based design
- Highly customizable: colors, opacity, displacement, etc.
- Integrated with `ScrollController` for programmatic control
- Supports various scrollable widgets like `ListView`, `GridView`, and `CustomScrollView`
- Easy installation and usage
- Prebuilt example project for quick testing and understanding

## Contributing

Contributions are welcomed for this project. Please review the [contributing guidelines](https://github.com/thisisyoussef/Liquid-Pull-To-Refresh/blob/master/CONTRIBUTING.md) and [code of conduct](https://github.com/thisisyoussef/Liquid-Pull-To-Refresh/blob/master/CODE_OF_CONDUCT.md) before making any changes or submitting a pull request. For any questions or issues, please open an issue on GitHub.

## License

This project is licensed under the MIT License. Please see the [license file](https://github.com/thisisyoussef/Liquid-Pull-To-Refresh/blob/master/LICENSE) for more information.

## Contact

If you have any questions or queries related to the project, feel free to reach out to the maintainer:

- Youssef: [GitHub](https://github.com/thisisyoussef)

Additionally, you can open an issue in the repository for any support requests or bug reports.