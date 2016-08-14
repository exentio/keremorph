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

    Pale colors just have 10% less saturation,
    except for black (20% less)

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

### How to install themes

That's pretty simple: just copy the folder inside `~/.themes` and apply it with `lxappearance` for GTK and `obconf` for Openbox

### How to install the Chromium/Google Chrome theme

Simply drop it inside the window

### How to install the Sublime Text 3 theme

If you don't have the Boxy theme, or you don't have any mod for it, simply drag `Boxy Theme.sublime-package` inside`/home/ex/.config/sublime-text-3/Installed Packages`.  
But if you already have it and you modded it, this gets trickier:  
* Extract the original theme (exactly like you would do with a .zip), and also this modded version  

* Go inside the modded theme's folder, and copy (from the modded's folder into the original's):   
  * `Boxy Keremorph.sublime-theme` in the root.  
  * `schemes/Boxy Keremorph.tmTheme` inside the`schemes` folder.  
  * `assets/specific/keremorph` inside the `assets/specific` folder.  

* Go in the root of the modded's folder and select all (`CTRL + A`), and compress everything in a zip

* Rename the zip `Boxy Theme.sublime-package`

* Apply the theme inside Sublime
