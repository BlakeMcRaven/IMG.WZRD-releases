# IMG.WZRD

A fast image viewer and editor for Windows.

- Opens 4K and 8K pictures in about half a second.
- Quick export: resize, change format and quality, pack channels for game textures.
- Inspect a file's metadata, read text in it, search your folders for look-alikes.
- Editor mode with layers, 83 effects and AI-assisted edits through your own AI account.
- Translate text in a picture, right on the picture.

## Download

Get the newest installer from the [latest release](https://github.com/BlakeMcRaven/IMG.WZRD-releases/releases/latest).

It installs for your user account only and needs no administrator rights. Windows 10 or
11, 64-bit. To remove it, use **Apps & features** like any other program; your own
settings and data are kept.

### Windows will warn you the first time

The installer is not code-signed yet, so Windows SmartScreen shows "Windows protected
your PC". Choose **More info**, then **Run anyway**. You can check the download first:
each release lists the installer's SHA-256, and this command prints the same value for
the file you downloaded:

```
certutil -hashfile IMG.WZRD-Setup-0.9.1.exe SHA256
```

## What it sends, and when

Nothing, until you ask. IMG.WZRD goes online only when you press a button that says so:

- **AI features** send the picture (rebuilt from its pixels, so without its metadata)
  and your request to the AI service you chose, using your own account or key.
- **Search the Web** sends the picture to the search service you chose.
- **Check for updates** reads one small file from this page. A once-a-day check exists
  and is switched off unless you switch it on.

Keys are stored in Windows Credential Manager, never in a file.

## Updates

In the app, click the **IMG.WZRD** name in the top bar, then **Check for updates**.

## Licences

IMG.WZRD is built with PhotoCraft's editing engine (MIT or Apache-2.0), ExifTool, egui
and other open-source libraries. Their licence texts and the full list are installed
beside the program, in the `licenses` folder.
