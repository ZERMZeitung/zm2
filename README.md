# zm2 -- The next-gen tool for managing ZERM articles

After struggling with maintaining [zm1](https://github.com/ZERMZeitung/zm1), with
the adoption of [jasmin](https://github.com/ZERMZeitung/jasmin) we have decided
to get a completely new tool to go alongside it.

`zm`'s role has changed: It now maintains a list of articles contained within
the `articles.csv` file and a list of drafts contained in the `drafts.csv` file.

## Usage

`zm` commands are all one letter. If you want to, you can still type them out though.

```sh
zm n(ew)     # Make a new draft.
zm e(dit)    # Edit a draft of an entry.
zm p(ublish) # Finalize/publish a draft.
zm P(DF)     # Generate a GA PDF
```

## Dependencies

- a posix system (`ls`, `wc`, `grep`, `sed`, `touch`, `cut`, `awk`, `tail`, `nl`, `echo`, `rev`, `mv`, `tr`)
- `iconv`
- `bash`
- a working `$EDITOR` (or, if `$EDITOR` is not set, `vi`)

## Installing

Just drop `zm` somewhere in a `bin` folder that's in your `PATH`
(or add the `zm2` folder to the `PATH`).

```sh
cp -f zm ~/.local/bin/
```
