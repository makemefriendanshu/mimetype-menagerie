----------------
Mimetypes to add
----------------

- `application`
    - [x] [`application/rtf`](media-types/application/rtf/) Rich Text Format ([`.rtf`](https://en.wikipedia.org/wiki/Rich_Text_Format))
    - [x] [`application/zip`](media-types/application/zip/) Zip file (`.zip`)
    - [x] [`application/x-compressed-tar`](media-types/application/x-compressed-tar/) Gzipped tar file (`.tar.gz`)
    - [ ] [DAISY e-book files](https://bugs.freedesktop.org/show_bug.cgi?id=91873)
    - [ ] `application/x-iso9660-image` ISO disk image ([`.iso`](https://en.wikipedia.org/wiki/ISO_image))
        - Hard to find files of reasonable size.
    - [ ] `application/x-dbf` dBASE database files ([`.dbf`](https://en.wikipedia.org/wiki/.dbf))
    - [ ] `application/vnd.ms-cab-compressed` Microsoft Windows Cabinet archive format ([`.cab`](https://en.wikipedia.org/wiki/Cabinet_%28file_format%29)) 
    - [ ] `application/x-font-ttf` TrueType font files ([`.ttf`](https://en.wikipedia.org/wiki/TrueType))
    - [ ] `application/sla` Stereolithography CAD file ([`.stl`](https://en.wikipedia.org/wiki/STL_%28file_format%29))
- `audio`
    - [ ] `audio/x-xm` Extended module tracker audio format ([`.xm`](https://en.wikipedia.org/wiki/XM_%28file_format%29))
- `image`
    - [x] `image/gif` An animated gif (current examples are static).
- `text`
    - [`text/plain`](media-types/text/plain/)
        - [ ] INI config files [`.ini`](https://en.wikipedia.org/wiki/INI_file)
        - [ ] [fstab](https://en.wikipedia.org/wiki/Fstab) file
        - [ ] debian `.dsc` files
    - `text/calendar`
        - [ ] iCal files ([`.ics`](https://en.wikipedia.org/wiki/ICalendar))
    - `text/csv`
        - [ ] [RFC 4180](https://tools.ietf.org/html/rfc4180) compliant files.
        - [ ] `.csv` files that are entirely numeric
        - [ ] `.csv` files with quoting
        - [ ] `.csv` files with semicolon delimiters and commas as decimal marks.
    - [ ] `text/x-apt-sources-list` (sources.list file for Debian)
        - https://www.debian.org/doc/debian-policy/ch-controlfields.html#s-controlsyntax

----------
Validation
----------

- [x] Check for broken URLs.
- [ ] Change JSON so that each file can have multiple URLs.
- [x] Check that each file is in the folder corresponding to its mimetype.
- [ ] List of SHA1 checksums to avoid re-downloading.
    - [ ] Even better, make zsync control files.
