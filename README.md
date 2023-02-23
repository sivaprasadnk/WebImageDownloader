## WebImageDownloader

Use this package to download / save images to your computer locally, when run in web.


## Getting started


Add this to your package's `pubspec.yaml` file

```yaml
dependencies:
  web_image_downloader: ^1.0.1
```

## Usage


First, you just have to import the package using:

```dart
import 'package:web_image_downloader/web_image_downloader.dart';
```

Then , wrap the required [image] widget with RepaintBoundary widget and pass a global key to it.

```dart
  RepaintBoundary(
      key: globalKey,
      child: Image.asset('assets/image.png'),
    ),
```

Finally , call the function as below,  by passing the global key and a required fileName.

```dart
  await WebImageDownloader.downloadImage(globalKey, 'image.png');
```

## Contributing
Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.