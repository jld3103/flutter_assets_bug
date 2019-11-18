# flutter_assets_bug
Example for flutter copying file to the build assets which is not in the assets.
Run:
```bash
flutter build web
cat build/web/assets/some_random_folder/file.txt
# -> this should not be copied
flutter clean
flutter build bundle
cat build/flutter_assets/some_random_folder/file.txt
# -> this should not be copied
```