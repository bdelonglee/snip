#### NUKE Textnode upstream filename
## CMD
[join [lrange [split [file tail [knob [topnode].file]] _ ] 0 3 ] _]


#### NUKE Textnode upstream dirpath + _ + basename
## CMD
[lindex [split [knob [topnode].file] /] 7]_[join [lrange [split [file tail [knob [topnode].file]] _ ] 0 3 ] _]


