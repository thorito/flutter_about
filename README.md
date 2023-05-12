# About Custom

Displays an About dialog, which describes the application.

<img alt="Example" src="https://raw.githubusercontent.com/DavBfr/flutter_about/master/example.jpg">

[![Buy Me A Coffee](https://bmc-cdn.nyc3.digitaloceanspaces.com/BMC-button-images/custom_images/orange_img.png "Buy Me A Coffee")](https://www.buymeacoffee.com/JORBmbw9h "Buy Me A Coffee")

## Usage

To use this plugin, add `about_custom` as a [dependency in your pubspec.yaml file](#-installing-tab-).

## Example

```
  showAboutPage(
    context: context,
    values: {
      'version': '1.0',
      'year': DateTime.now().year.toString(),
    },
    applicationLegalese: 'Copyright © Thorito, {{ year }}',
    applicationDescription: const Text(
        'Displays an About dialog, which describes the application.'),
    children: const <Widget>[
      MarkdownPageListTile(
        icon: Icon(Icons.list),
        title: Text('Changelog'),
        filename: 'CHANGELOG.md',
      ),
      LicensesPageListTile(
        icon: Icon(Icons.favorite),
      ),
    ],
    applicationIcon: const SizedBox(
      width: 100,
      height: 100,
      child: Image(
        image: AssetImage('assets/icon.webp'),
      ),
    ),
  );
```
