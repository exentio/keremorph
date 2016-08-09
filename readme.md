# Keremorph Color Scheme

Color scheme born in a day filled with boredrom, the 9 August 2016.

![alt text](https://raw.githubusercontent.com/exentio/keremorph/master/preview.png "Preview")

### Colors

    Background:     #173559
    Text/Fore:      #E3D1D1
    Black:          #323C51
    Red:            #A43C38
    Green:          #499860
    Yellow:         #CD8D4C
    Blue:           #326E95
    Magenta:        #A6346B
    Cyan:           #32939A
    White:          #E8D5D5
    
    Pale colors just have 10% less saturation

### How to add the scheme in .Xresources

I decided to use a modular approach, inspired by [dkeg](https://github.com/dkeg) (this means keremorph is compatible with his schemes), but this works only with 8+1 colors.
To add the scheme to .Xresources, simply paste this into the file, after other settings, and remove the previous colors if present:

    #include <keremorph/keremorph>        ! - Change this if the repo isn't inside ~/keremorph

    ! Colors
    *background:   bg
    *foreground:   fg
    *cursorColor:  cyn

    *color0:      blk
    *color8:      bblk
    *color1:      red
    *color9:      red
    *color2:      grn
    *color10:     grn
    *color3:      ylw
    *color11:     ylw
    *color4:      blu
    *color12:     blu
    *color5:      mag
    *color13:     mag
    *color6:      cyn
    *color14:     cyn
    *color7:      wht
    *color15:     wht

Instead, if you prefer 16 colors, use this (modular, but doesn't work with dkeg colors without editing his files)

    ! Colors
    *background:   bg
    *foreground:   fg
    *cursorColor:  cyn

    *color0:      blk
    *color8:      bblk
    *color1:      red
    *color9:      bred
    *color2:      grn
    *color10:     bgrn
    *color3:      ylw
    *color11:     bylw
    *color4:      blu
    *color12:     bblu
    *color5:      mag
    *color13:     bmag
    *color6:      cyn
    *color14:     bcyn
    *color7:      wht
    *color15:     bwht

### How to install the Openbox theme

That's pretty simple: just copy the `openbox-3` folder inside `~/.themes/keremorph` and apply it with `obconf`
