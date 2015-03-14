##Themes for [Documentation generator](https://github.com/Whyounes/gDoc)

Themes for the documentation generator must contain two files:

- `theme.yml`: This file contain your theme definition. It must contain a `name` attribute. The `assets` attribute is optional and contain a list of file that will be copied to the build output.
- `page.twig`: This file is called for every page of your doc and you will have access to the following variables:
 - `rootPath`: contain the current root folder, if you have multiple versions of your documentation it will be `master`, `4.2`, etc.
 - `content`: HTML parsed content.
 - `assets`: List of assets as specified in your theme file.
 - `filename`: The current parsed file name.
 - `navigation`: The list of navigation specified on your `doc.yml`.