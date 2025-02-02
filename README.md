# October CMS Twig Highlighter

This package adds syntax definitions for the [October CMS](https://docs.octobercms.com/2.x/markup/templating.html) Twig engine. Support is available for [Sublime Text](https://www.sublimetext.com/) and [Visual Studio Code](https://code.visualstudio.com/).

## Visual Studio Code

### How to install with VS Code

Search for **October Twig** and install the package. You can then select "October CMS Template" from the available syntax list.

If you would like the INI syntax to be enabled, `##` must be at the beginning of the template file. For example:

```
##
url = "/blog"
layout = "default"
==
<?
function onStart() { /* ...*/ }
?>
==
<h1>Page Title</h1>

{% for post in posts %}
    <h4>{{ post.title }}</h4>
    {{ post.content}}
{% endfor %}
```

#### How to Contribute

- Intall this extension
- Open the `%USERPROFILE%\.vscode\extensions` directory
- Modify the extension files
- Reload the window to test

## Sublime Text

Uses `.sublime-syntax` files that works with Sublime Text 3 and newer.

### How to install with [Sublime Package Control](http://wbond.net/sublime_packages/package_control)

Search for **October Twig** and install it, it's just that simple.

Restart Sublime Text after you install this package.

### Sublime Text Manual Install

- Download or clone this repository into [install-dir]/Packages/october-twig
- Restart Sublime Text.

#### How to Contribute

- To test a local version of the highlighter first uninstall the highlighter from package control.
- Follow the manual installation process by cloning the repo into your packages directory.
- Restart Sublime Text.
- Open up the '[install-dir]/Packages/october-twig' folder into a new Sublime Text project.
- Open up the `october-twig.sublime-syntax` file and make changes.
- Provided is a `test.htm` file that holds most of the common uses for testing the regex, use this to verify your changes before and after you make them to ensure the changes you make do not break anything.
- Send a pull request with a single change per request.

## Thanks

- Thanks @dqsully for the original [October CMS Template language](https://github.com/dqsully/octobercms-template-language) package.
- Thanks @Anomareh for the [PHP-Twig TextMate bundle](https://github.com/Anomareh/PHP-Twig.tmbundle) used to source the Twig functions.
