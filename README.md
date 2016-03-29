# WSH Javascript Compressor

Javascript compression script for Windows Script Host and command line.

Generate minified version of javascript file by removing line breaks, tabs, extra spaces and semicolons before closing braces.

The name of the compressed file is supplemented by the suffix `.min`.

Script correctly process files with multiple extensions. For example: `source.core.js` converts to `source.core.min.js`.

## Usage

You can use this script in two ways:

1. Drag your javascript file over the compressor script and in the directory with the source file appears minified version.
2. Run compression from the command line (this method allows to set advanced options).

**Command line syntax:** `compressor.wsf sourcePath [newPath]`

**Command examples:**

```
compressor.wsf source.js                                            // source.min.js
compressor.wsf C:\path\source.js                                    // C:\path\source.min.js
compressor.wsf C:\path\source.js custom_name.js                     // C:\path\custom_name.js
compressor.wsf C:\path\source.js X:\custom_dir\                     // X:\custom_dir\source.min.js
compressor.wsf C:\path\source.js X:\custom_dir\custom_name.js       // X:\custom_dir\custom_name.js
compressor.wsf source.js X:\custom_dir\                             // X:\custom_dir\source.min.js
compressor.wsf source.js X:\custom_dir\custom_name.js               // X:\custom_dir\custom_name.js
compressor.wsf source.js custom_name.js                             // custom_name.js
```

**Warning:** Don't forget to wrap the file path into quotes if it contains spaces.

## Links

- Project site: http://github.com/alexkudrow/wsh-javascript-compressor
- Author: Alex Kudrow (http://github.com/alexkudrow)
- Based on packer script by Dean Edwards (http://dean.edwards.name/packer)

## License

Distributed under the terms of the [MIT license](https://opensource.org/licenses/MIT)

© 2016 Alex Kudrow (http://github.com/alexkudrow)
