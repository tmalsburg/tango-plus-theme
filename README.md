tango-plus-theme
================

Color theme for Emacs loosely based on the tango palette.  As all
themes, this is a work in progress.  The basis for this theme was the
tango theme that is part of Emacs 24.  However, some colors where
added to increase contrast.  Also, support was added for evil, org
mode, mu4e, and helm.

## Installation

Have Emacs 24 or higher.  Put the file tango-plus-theme.el in a
directory included in your load-path.  Add the following line to your
startup file (typically init.el):

    (load-theme 'tango-plus t)

## Design principles

Use colors sparingly.  Use colors as semantic annotation: the meaning
of a color should be consistent across buffers and languages.  Also,
the meaning of a color should be self-explanatory to the extent
possible.  For example, a red background is for errors (flyspell) and
stuff that was (ediff) or is going to be deleted (search & replace in
evil).  Green background is for matches (isearch) or inserted material
(ediff).  Selections are marked with yellow background, think text
marker.  All neutral types of highlights use a light grey for the
background (sentence-highlight-mode, hl-line-mode,
show-paren-match).  Foreground colors: Blue is used for keywords
(electric sparks).  Newly defined stuff like functions is red (hot
from the forge).  String constants are brown like burned
bricks.  Comments are grey.
