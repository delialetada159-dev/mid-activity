# Upload this project to GitHub without installing Flutter

You only need a browser to upload the source files. Flutter is needed to run/test the app, not to publish the code on GitHub.

1. Download `Product_Store_Flutter_GitHub_Ready.zip` and choose **Extract All**.
2. Open your GitHub repository in your browser.
3. Click **Add file → Upload files**.
4. In File Explorer, open the extracted `Product_Store_Flutter_GitHub_Ready` folder. Select the items inside it: `lib`, `pubspec.yaml`, `.gitignore`, `README.md`, and this guide. Drag the selected items into the GitHub upload area. If folder drag-and-drop does not work in your browser, upload the files through a local Git workflow or GitHub Desktop.
5. Enter a commit message such as `Add Product Store Flutter source code` and click **Commit changes**.
6. Refresh the repository. At its top level, you should see `lib`, `pubspec.yaml`, `README.md`, and `.gitignore`.

**Important:** Do not upload just the ZIP when your instructor needs to inspect your source code. Upload the extracted contents. Keep your existing ZIP as an optional backup attachment.

## To run the app later

A computer with Flutter installed is required. From the project folder run:

```bash
flutter create .
flutter pub get
flutter analyze
flutter run
```
