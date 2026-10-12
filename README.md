# Product Store Flutter App

A simple Flutter REST API project for practicing `FutureBuilder`, `StreamBuilder`, and reusable UI components. It uses the DummyJSON Products API and does not require an API key.

## Features

- **Products screen:** loads 10 products with `FutureBuilder`.
- **Live Product screen:** uses `StreamBuilder` to load a new product every five seconds.
- Loading, retry, error, and empty states.
- Reusable product cards and text components, organized with an atomic-design-inspired folder structure.

## API

- Product list: <https://dummyjson.com/products?limit=10>
- Single product: <https://dummyjson.com/products/1>
- Documentation: <https://dummyjson.com/docs/products>

An internet connection is needed for API data.

## Project structure

```text
lib/
├── main.dart
├── models/
│   └── product.dart
├── services/
│   └── product_services.dart
└── ui/
    ├── atoms/
    │   └── app_text.dart
    ├── organism/
    │   └── product_card.dart
    ├── pages/
    │   ├── single_fetch.dart
    │   └── stream_page.dart
    └── templates/
        └── product_templates.dart
pubspec.yaml
README.md
.gitignore
```

## About running the app

This repository contains the Flutter/Dart source code and package configuration. You do **not** need Flutter installed just to upload or view the source on GitHub. To run the app, a computer with the Flutter SDK is required.

After installing Flutter, open this project folder in VS Code or a terminal and run:

```bash
flutter create .
flutter pub get
flutter analyze
flutter run
```

`flutter create .` generates the platform folders (such as `android` and `web`) for this source-only starter project.

## Uploading on GitHub without Flutter

1. Download and extract the ZIP package.
2. Open your GitHub repository and click **Add file → Upload files**.
3. Open the extracted `Product_Store_Flutter_GitHub_Ready` folder on your computer. Drag its contents (including the `lib` folder and the files `pubspec.yaml`, `README.md`, and `.gitignore`) into GitHub's upload area. Do not upload only the ZIP if your instructor needs to see the code files.
4. Enter a commit message such as `Add Product Store Flutter source code`.
5. Click **Commit changes**.

GitHub's browser upload supports up to 100 files at a time and a 25 MiB per-file limit. See the [official GitHub instructions](https://docs.github.com/en/repositories/working-with-files/managing-files/adding-a-file-to-a-repository).
