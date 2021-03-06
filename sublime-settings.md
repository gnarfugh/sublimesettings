###My sublime User Settings

```
{
	"Seti_show_group_arrows": true,
	"Seti_sidebar_font_size_12": true,
	"caret_extra_bottom": 3,
	"caret_extra_top": 3,
	"caret_extra_width": 2,
	"channels":
	{
		"dec": "\\d{1,3}",
		"empty": "",
		"float": "(?:[0|1])|(?:[1][\\.]?[0]*)|(?:[0]?[\\.]\\d*)",
		"hex1": "[0-9a-fA-F]",
		"hex2": "[0-9a-fA-F]{2}",
		"hue": "dec",
		"lightness": "perc",
		"perc": "\\d{1,3}[%]",
		"saturation": "perc",
		"value": "perc"
	},
	"color_scheme": "Packages/User/Dracula (SL).tmTheme",
	"convert_util_path": "convert",
	"default_keybindings": true,
	"enabled": true,
	"file_exts":
	[
		".css",
		".sass",
		".scss",
		".less",
		".styl",
		".html",
		".js",
		".sublime-settings",
		".tmTheme",
		".erb",
		".haml",
		".back",
		".py",
		".md"
	],
	"font_size": 17,
	"formats":
	{
		"@named":
		{
			"description": "Named css colors"
		},
		"@varless":
		{
			"description": "Less variables: @a-b-c"
		},
		"@varsass":
		{
			"description": "Sass variables: $a-b-c"
		},
		"@varstyl":
		{
			"description": "Styl variables: a-b-c"
		},
		"@varstyldollar":
		{
			"description": "Styl variables: $a-b-c"
		},
		"hex3":
		{
			"after": "hex4",
			"description": "Hex 0xRGB color format",
			"regex": "0x(?P<R>hex1)(?P<G>hex1)(?P<B>hex1)\\b",
			"white": "0xFFF"
		},
		"hex4":
		{
			"after": "hex6",
			"description": "Hex 0xRGBA color format",
			"regex": "0x(?P<R>hex1)(?P<G>hex1)(?P<B>hex1)(?P<A>hex1)\\b",
			"white": "0xFFFF"
		},
		"hex6":
		{
			"after": "hex8",
			"description": "Hex 0xRRGGBB color format",
			"regex": "0x(?P<R>hex2)(?P<G>hex2)(?P<B>hex2)\\b",
			"white": "0xFFFFFF"
		},
		"hex8":
		{
			"description": "Hex 0xRRGGBBAA color format",
			"regex": "0x(?P<R>hex2)(?P<G>hex2)(?P<B>hex2)(?P<A>hex2)\\b",
			"white": "0xFFFFFFFF"
		},
		"hsl":
		{
			"description": "hsl(hue 0..255, s%, v%) color format",
			"regex": "hsl[(][ ]*(?P<R>hue)[ ]*[,][ ]*(?P<G>saturation)[ ]*[,][ ]*(?P<B>lightness)[ ]*[)]",
			"white": "hsl(0, 0%, 100%)"
		},
		"hsla":
		{
			"description": "hsla(hue 0..255, s%, v%, alpha 0.0 .. 1.0) color format",
			"regex": "hsla[(][ ]*(?P<R>hue)[ ]*[,][ ]*(?P<G>saturation)[ ]*[,][ ]*(?P<B>lightness)[ ]*[,][ ]*(?P<A>float)[ ]*[)]",
			"white": "hsla(0, 0%, 100%, 1.)"
		},
		"hsv":
		{
			"description": "hsv(hue 0..255, s%, v%) color format",
			"regex": "hsv[(][ ]*(?P<R>hue)[ ]*[,][ ]*(?P<G>saturation)[ ]*[,][ ]*(?P<B>value)[ ]*[)]",
			"white": "hsv(0, 0%, 100%)"
		},
		"hsva":
		{
			"description": "hsva(hue 0..255, s%, v%, alpha 0.0 .. 1.0) color format",
			"regex": "hsva[(][ ]*(?P<R>hue)[ ]*[,][ ]*(?P<G>saturation)[ ]*[,][ ]*(?P<B>value)[ ]*[,][ ]*(?P<A>float)[ ]*[)]",
			"white": "hsva(0, 0%, 100%, 1.)"
		},
		"rgb":
		{
			"description": "rgb(255,255,255) color format",
			"regex": "rgb[(][ ]*(?P<R>dec)[ ]*[,][ ]*(?P<G>dec)[ ]*[,][ ]*(?P<B>dec)[ ]*[)]",
			"white": "rgb(255, 255, 255)"
		},
		"rgb_array":
		{
			"description": "[r, g, b] color format, where each channel can be int(0..255) or float(0. .. 1.) or percentage (0..100)%. For example: [255, 100%, 1., 255]",
			"regex": "[\\[][ ]*(?P<R>dec|perc|float)[ ]*[,][ ]*(?P<G>dec|perc|float)[ ]*[,][ ]*(?P<B>dec|perc|float)[ ]*[\\]]",
			"white": "[255, 255, 255]"
		},
		"rgba":
		{
			"description": "rgba(255,255,255,1) color format",
			"regex": "rgba[(][ ]*(?P<R>dec)[ ]*[,][ ]*(?P<G>dec)[ ]*[,][ ]*(?P<B>dec)[ ]*[,][ ]*(?P<A>float)[ ]*[)]",
			"white": "rgba(255, 255, 255, 1)"
		},
		"rgba_array":
		{
			"description": "[r, g, b, a] color format, where each channel can be int(0..255) or float(0. .. 1.) or percentage (0..100)%. For example: [255, 100%, 1., 255]",
			"regex": "[\\[][ ]*(?P<R>dec|perc|float)[ ]*[,][ ]*(?P<G>dec|perc|float)[ ]*[,][ ]*(?P<B>dec|perc|float)[ ]*[,][ ]*(?P<A>dec|perc|float)[ ]*[\\]]",
			"white": "[255, 255, 255, 255]"
		},
		"sharp3":
		{
			"after": "sharp4",
			"description": "Hex #RGB color format",
			"regex": "(?<!&)#(?P<R>hex1)(?P<G>hex1)(?P<B>hex1)(?!\\w)",
			"white": "#FFF"
		},
		"sharp4":
		{
			"after": "sharp6",
			"description": "Hex #RGBA color format",
			"regex": "(?<!&)#(?P<R>hex1)(?P<G>hex1)(?P<B>hex1)(?P<A>hex1)(?!\\w)",
			"white": "#FFFF"
		},
		"sharp6":
		{
			"after": "sharp8",
			"description": "Hex #RRGGBB color format",
			"disable_exts": ".py",
			"regex": "(?<!&)#(?P<R>hex2)(?P<G>hex2)(?P<B>hex2)(?!\\w)",
			"white": "#FFFFFF"
		},
		"sharp8":
		{
			"description": "Hex #RRGGBBAA color format",
			"disable_exts":
			[
				".py"
			],
			"regex": "(?<!&)#(?P<R>hex2)(?P<G>hex2)(?P<B>hex2)(?P<A>hex2)(?!\\w)",
			"white": "#FFFFFFFF"
		}
	},
	"ha_icons": false,
	"ha_style": "default",
	"highlight_line": true,
	"icons": true,
	"ignored_packages":
	[
		"Vintage"
	],
	"overlay_scroll_bars": "enabled",
	"style": "default",
	"tab_size": 2,
	"theme": "Seti.sublime-theme",
	"translate_tabs_to_spaces": true
}
