# ScalaScript extension for Visual Studio Code

A [Visual Studio Code](https://code.visualstudio.com) extension for [Scala Inc](https://www.scala.com)'s ScalaScript digital signage scripting language. 

## Features

This extension provides syntax highlighting including:
- ScalaScript structural elements such as **Group** and **Sequence** list introducers
- Variable types such as **Integer**, **Boolean**, and **String**, etc.
- Script control keywords such as **If**, **Goto**, **Use**, **Hotkey**, etc.
- Modifiers such as **Template**, **External**, **Optional**, and **Disabled**
- Line comments

## Requirements

Developed and tested with Visual Studio Code 1.31. Tested using various built-in themes and some theme extensions.

## Extension Settings

None currently.

## Notes
- Any trademarks and logos are the property of Scala Inc. or the trademark/logo owners
- The author is not affiliated with scala.com.

## Other Scala-Related Tips

The [Log File Highlighter extension](https://marketplace.visualstudio.com/items?itemName=emilast.LogFileHighlighter) is handy for viewing Scala Designer and Player log files. Add the following custom patterns to your `settings.json` for optimal viewing. The final pattern is used to dim the end-of-line timecodes... make sure its `foreground` color is low-contrast to your background. (These values are chosen for a light background.)

```
    "logFileHighlighter.customPatterns": [
        {
            "pattern": "SCALA",
            "foreground": "#AA0088"
        },
        {
            "pattern": "RUNIC",
            "foreground": "#00AA00"
        },
        {
            "pattern": "NETIC",
            "foreground": "#0000AA"
        },
        {
            "pattern": "ERROR Problem [0-9]+, Error [0-9.]+:",
            "foreground": "#CC0000"
        },
        {
            "pattern": "\\|\\([0-9][0-9][0-9][0-9][0-9][0-9][0-9][0-9][0-9][0-9][0-9][0-9][0-9][0-9][0-9][0-9]\\)",
            "foreground": "#CCCCCC"
        }
    ],
```

## Known Issues

Block comments (/* comment */) are not currently highlighted.

## Release Notes

Users appreciate release notes as you update your extension.

### 1.0.0

Initial release.
