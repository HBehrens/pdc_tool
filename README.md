# pdc_tool

Command-line interface to work with Pebble Draw Command (PDC) files. With `pdc_tool` you can convert SVGs to PDCs, render PDCs as PNGs or rendering SVGs directly while producting pixel-perfectly the same output the original Pebble (1bit b&w) or Pebble Time (64 colors) with or without anti-aliasing would.

![Screenshot pdc_tool in the terminal](screenshot.png)

> [!NOTE]
> This is an early version with known limitations. While this tool should not cause any harm, it may fail in (un-)expected ways.

Download the platform-specific binary from [pdc_tool/releases](https://github.com/HBehrens/pdc_tool/releases).

## Future Plans
* [ ] Introduce command `pdc` to actually save a PDC
* [ ] Emit diagnostics during conversion
* [ ] Command `svg` to produce annotated output (incl. diagnostics)
* [ ] Support for bezier curves

## Permissions on macOS

You may see a dialog "Apple could not verify “pdc_tool” is free of malware that may harm your Mac or compromise your privacy." when trying to run `pdc_tool` after downloading it. You can either click on that dialog's (?) icon and follow the instructions provided or clear the automatically added quarantine flag from the terminal via `xattr -d com.apple.quarantine ~/Downloads/pdc_tool`.
