---
layout: post
title: "Notes On JavaScript ID3V2.4 Parser"
date: 2013-11-20 15:36:25 -0600
comments: false
categories: [JavaScript]
---
In order to learn JavaScript, in addition to reading books I started working on a ID3 parser. I decided to write a ID3 parser initially focusing on parsing 2.4 tags. In summary, ID3V2.4 has a 10 byte header followed by 4 bytes of optional extended header with most integers encoded as SynchSave integers. Frames start immediately after header with 10-byte frame header. Frame header is composed of 4 consecutive ISO-8859-1 charaters from A-Z and 0-9 followed by 1 byte of size and 2 bytes of flags. Textual frames all starts with 'T' and the byte immediately after frame header indicates string encoding (ISO-8859-1, UTF-16, UTF-16BE, UTF-8).


ID3V2.4.0 documentations:

- [ID3v2.4.0-structure](http://id3.org/id3v2.4.0-structure)
- [ID3v2.4.0-frames](http://id3.org/id3v2.4.0-frames)

Existing projects:

- [43081j/id3](https://github.com/43081j/id3)
- [JavaScript-ID3-Reader from Opera](https://github.com/aadsm/JavaScript-ID3-Reader)
- [LISP ID3 parser from "Practical Common LISP"](http://www.gigamonkeys.com/book/practical-an-id3-parser.html)


