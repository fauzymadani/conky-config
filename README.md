
# conky-config

a config for conky on linux.


## requirements

 - [JetBrains Mono Nerd Fonts](https://www.nerdfonts.com/font-downloads)
 - [3720 Nerd Fonts](https://www.nerdfonts.com/font-downloads)
 - [conky](https://github.com/brndnmtthws/conky)


## usage

you can clone this repo and replace the default conky config with this config. or you can copy raw code and paste the code to your `/etc/conky/conky.conf` .


## Installation

raw code. paste this config to your `/etc/conky/conky.conf`.


```conf
  conky.config = {
    alignment = 'top_middle',
	background = false,
	border_inner_margin = 15,
	border_width = 5,
	default_color = '5A5B3F',  --ffffff # grey 5f5f5f 3F3F3F 183149 3B3B3B 26211F
	double_buffer = true,
	draw_borders = false,
	draw_graph_borders = false,
	draw_outline = false,
	draw_shades = false,
	gap_x = 30,
	gap_y = 60,
	maximum_width = 650,
	double_buffer = true,
	override_utf8_locale = true,
    own_window = true,
    own_window_class = 'Conky',
    own_window_type = 'normal',
	own_window_transparent = false,
	own_window_hints = 'undecorated,below,skip_taskbar,skip_pager,sticky',
	own_window_argb_visual = true,
	own_window_argb_value = 0,
	text_buffer_size = 8000,
	total_run_times = 0,
	update_interval = 1,
	uppercase = false,
	use_xft = true,
	xftalpha = 1,
	short_units = false,
	font = 'Raleway:style=Light:pixelsize=16',
	color1 = '505139',
	color2 = '005929',
	color3 = '005929',
}
conky.text = [[

${font JetBrainsMono Nerd Font:weight=Light:size=78}${alignc}${time %I:%M}${font}

${goto 15}${font JetBrainsMono Nerd Font:weight=Light:size=28}${alignc} ${time %A %B %d}${font}
${alignc}${voffset 6}${offset 12}${font GE_Inspira:pixelsize=14}${color 86877A}HD ${offset 9}$color${fs_free /} / ${fs_size /}${offset 30}${color 86877A}RAM ${offset 9}$color$mem / $memmax${offset 30}${color 86877A}CPU ${offset 9}$color${cpu cpu0}%
${alignc}       __________________________________________________________________________

${font 3270 Nerd Font:pixelsize=25}${alignc}${color1}php is suck${color}
]]
```

## functionality
you can customize the color by editing the color section. `color1 = '505139',
	color2 = '005929',
	color3 = '005929',`

the font on the `{font JetBrainsMono Nerd Font:`
you have to install this font widely for your system, you can change the font.
## icon
for the icon, read conky documentation.

## screenshots
![Screenshot from 2024-07-15 11-57-44](https://github.com/user-attachments/assets/7cc73403-aab0-406d-8f1c-adb66caf2cb6)

