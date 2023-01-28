---
title: "Batch renaming files"
date: "2015-07-11"
---

I needed to batch rename some files

brew install rename

To test run it

rename -n -e 's/-.\*-/\_/'  \*.png

Remove the -n to perform it

rename -e 's/-.\*-/\_/'  \*.png

I wanted to remove the following -portrait

rename -d -portrait \*

Thanks to

http://stackoverflow.com/questions/24102974/mac-os-x-terminal-batch-rename

http://superuser.com/questions/398709/mass-remove-file-prefix-on-a-mac
