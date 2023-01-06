# UnleashX Manual

UnleashX is one of the most popular custom dashboard for the first generation Microsoft Xbox (ogxbox). As its author described:

> UnleashX is an Xbox Application/Game launcher, with a few other features thrown in. I've designed UnleashX with safety in mind. I intentionally left out any feature that could potentially render your xbox useless, except for the HD formatting.

Unfortunately there is not much documentations left about it. Void with the volatile nature of internet, or perhaps stored deep down on internet archive site.

There is this one manual in PDF that quite comprehensive but a little bit hard to read. So I took the effort to rewrite (reformat?) it to make it easy on the eyes and probably can be exported to another ebook formats out there.
As for now the focus is on PDF, but I think the EPUB generated is quite readable.

### Dependencies

- pandoc
- xelatex
- texlive-extra-utils
- texlive-xetex

### How to create

- PDF

  ```sh
  ./create pdf
  ```

- EPUB

  ```sh
  ./create epub
  ```

### How to

- Change fonts
  Add font's name to [UnleashX.md](UnleashX.md?plain=1#L1) metadata. \
  Example:

  ```md
  mainfont: DejaVuSerif
  sansfont: DejaVuSans
  monofont: DejaVuSansMono
  mathfont: TeXGyreDejaVuMath-Regular
  ```

- Change syntax highlighting
  Change highlight style in [create](create#L84) with following styles:
  ```sh
  $ pandoc --list-highlight-styles
  pygments
  tango
  espresso
  zenburn
  kate
  monochrome
  breezedark
  haddock
  ```

### License

License for this repository is as stated in [LICENSE](LICENSE) file, except the source folder contents.
Documents inside source folder are belong to its author(s) and included here for the sake of preservation.
