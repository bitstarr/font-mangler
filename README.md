# Webfont Mangler

Since the webfont generator of fontsquirrel is not reliable anymore, we need to subset our webfonts by our selfs. So here is this tool!

Basically it's litte convinience helper to use [glyphhanger](https://github.com/filamentgroup/glyphhanger/).

You will to install `fonttools`, `brotli` and `zopfli` via python.

```
pip install fonttools
pip install brotli
pip install zopfli
```

## Usage

Put your source font filesd in the ``src`` folder. Now run

```
npm run subset
```

and find the processed files in the folder ``webfonts``.

## Configuration

In ``package.json`` is a config section. There you can setup the folders and the unicode range you want to use to subset. The default subset is for typical german text and includes:

* numbers, punctuation, diacritical, €
* de, pl, cz, it, fr
* latin-1