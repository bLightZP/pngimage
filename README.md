# pngimage
Portable Network Graphics Delphi 1.566  (24 November 2024)

This is a full, open sourced implementation of png in Delphi
It has native support for most of png features including the
partial transparency, gamma and more.

# Created by
Gustavo Huffenbacher Daud (gustavo.daud@terra.com.br)

# Some background
This widely used unit was no longer updated by its original author.

Unfotunately it still had a few bugs, so I decided to keep this repository up to date with all the fixes I've found since the last official release:

  Version 1.566
  2024-11-24   BUG 1     - Access violation with 1/2/4 bit transparent
                           png files. The source pointer calculation
                           was assuming 8bit at all times, resulting
                           in invalid memory access.
                           - Yaron Gur

  Version 1.565
  2023-11-07   BUG 1     - There was a possible access violation
                           when applying the alpha mask because an extra
                           byte was read that possible fell beyond the
                           end of the row of pixels
                           - Stijn Sanders


# Original repository
http://pngdelphi.sourceforge.net
