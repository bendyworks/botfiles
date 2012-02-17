# botfiles

	                          .coCO888888OCc.
	                      :oO@@@@@@@@@@@@@@@@o
	                   :C@@@@@@@@@@@@@@@@@@@@@:        C@Oo.
	                 c8@@@@@@@@@@@@@@@@@@@@@@@c       o@@@@@8o.
	               o@@@@@@@@@@@@@@@@@@@@@@@@@@     :cc@@@@@@@@@O:
	             c8@@@@@@@@@@@@Oc: .@@@@@@@@@o    .c:@@@@@@@@@@@@8:
	           .O@@@@@@@@@@@Ooccoo.8@@@@@@@@O    .o .cO@@@@@@@@@@@@O.
	         .c@@@@@@@@@@@Oc:.  o.O@@@@@@@@@.    ooc.   cO@@@@@@@@@@@o
	        :o@@@@@@@@@@O:     o.C@@@@@@@@@:     .coCoc.  .O@@@@@@@@@@O
	      .:o@@@@@@@@@@:      c:c@@@@@@@@@c         .cCCo:  .8@@@@@@@@@8
	     .:c@@@@@@@@@O       :c.@@@@@@@@@C             cCCo.  o@@@@@@@@@O
	    .c.@@@@@@@@@O       .o.8@@@@@@@@8      .o        cCC:  c@@@@@@@@@C
	   .o 8@@@@@@@@O        o.O@@@@@@@@@.     .@@@c       :oCc  c@@@@@@@@@:
	   o.c@@@@@@@@@.       o.o@@@@@@@@@:    : 8@@@@8c      .oCc  C@@@@@@@@8
	  cc 8@@@@@@@@o       cc.@@@@@@@@@o    o.O@@@@@@@O.     .CC:  @@@@@@@@@.
	 .C..@@@@@@@@@       .o 8@@@@@@@@O    c:o@@@@@@@@@@c     :Co  C@@@@@@@@o
	 co c@@@@@@@@O       o.c@@@@@@@@@.   c: .C@@@@@@@@@@o     oC: c@@@@@@@@C
	 Cc o@@@@@@@@C      cc 8@@@@@@@@c   :Co:  .8@@@@@@@@@:    :Cc :@@@@@@@@O
	.Cc c@@@@@@@@O     .C..@@@@@@@@@     :oCo.  O@@@@@@@@O    .Cc c@@@@@@@@O
	.Cc :@@@@@@@@8     co :@@@@@@@@O       cCC. .@@@@@@@@@    .Cc C@@@@@@@@o
	.Co  @@@@@@@@@:    Cc .@@@@@@@@@:       cCo o@@@@@@@@8    .C: @@@@@@@@@:
	 CC  C@@@@@@@@8   .Co  C@@@@@@@@@C.      Coo@@@@@@@@@c    :o C@@@@@@@@8
	 oC: .@@@@@@@@@o   oC:  8@@@@@@@@@@8OCooC@@@@@@@@@@@O     o:c@@@@@@@@@:
	 :Co  c@@@@@@@@@o  :Co.  O@@@@@@@@@@@@@@@@@@@@@@@@@O     :c:@@@@@@@@@C
	  oCc  C@@@@@@@@@C  cCo.  c@@@@@@@@@@@@@@@@@@@@@@@c     .co@@@@@@@@@8
	  .CC:  O@@@@@@@@@8: cCCc   cO@@@@@@@@@@@@@@@@@Oc      .oO@@@@@@@@@8
	   :CC:  C@@@@@@@@@@O..oCCc.   coO8@@@@@@@@OCc.       :O@@@@@@@@@@O
	    :CC:  c@@@@@@@@@@@O:.cCCoc:.     .....::.       :C@@@@@@@@@@@o
	     :CCc  .O@@@@@@@@@@@@Cc::cooCCooooocc.       :C8@@@@@@@@@@@8:
	      .oCo.  :8@@@@@@@@@@@@@8Co:..         .:cC8@@@@@@@@@@@@@@c
	        cCCc.  :O@@@@@@@@@@@@@@@@@@@8888@@@@@@@@@@@@@@@@@@@8c
	         .cCCc.  .C@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@C:
	           .cCCo:   :C8@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@8Cc.
	              :oCCo:.   coO@@@@@@@@@@@@@@@@@@@@@@8Coc..
	                .:oCCoc:.    :coCCOO8888OOCCoc:::::.
	                    .:coCCooc::..........::cccc.
	                         ..::cccoooocccc::.

## Problem Statement

We want a consistent set of dotfiles for setting up new machines when pairing, but we
all have different, subtle personal preferences.

## Usage

`~> wget $(http://url.to.botfiles.sh)`
`~> gem install oneonel`
`~> oneonel analyze`

### Backup

`~> oneonel backup` will prompt you to back up all of the dotfiles found in your $HOME directory. As of this moment oneonel does not support analysis on dotfiles sourced from within your existing dotfiles.

In order to make sure you get all of your dotfiles backed up you can `~> oneonel backup --with=bin,personal/bash_files,etc_dir`

### Modules

Modules are dotfiles that may include additional metadata to ensure they are loaded in a specific order, depend on other modules, and so on.

#### Listing

`~> oneonel ls` shows the list of available modules.

`~> oneonel ls --loaded` shows the list of currently loaded modules.

#### Loading

`~> oneonel load module_name`

#### Unloading

`~> oneonel unload module_name`


## Sensible Defaults

* TODO: what portions of dotmatrix are sensible and which aren't?

## User Profiles

* TODO: `oneonel decompose [filename]`