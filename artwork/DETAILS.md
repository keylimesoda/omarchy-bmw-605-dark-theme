# Theme details

| Role | Color |
| --- | --- |
| Background | `#080704` |
| Bar background | `#0f0b07` |
| Raised surface | `#1c150e` |
| Walnut selection | `#4a2816` |
| Accent and shell text | `#ff3900` |
| Terminal text | `#e7bd85` |
| Muted text | `#a8875f` |
| Bright terminal text | `#f3d5a8` |

## Color science

The 605 nm reference follows BMW’s classic orange-red instrument lighting, as described in [this interview with BMW interior designer Oliver Heilmer](https://www.autoblog.com/features/bmw-x4-toyota-tacoma-gauge-illumination).

The screen approximation uses [CIE 1931 2-degree observer data](https://cie.co.at/datatable/cie-1931-colour-matching-functions-2-degree-observer). At 605 nm, XYZ is `(1.0456, 0.5668, 0.0006)`. Add the minimum D65 white needed to enter the sRGB gamut, normalize the peak linear RGB channel, then apply the [sRGB transfer function](https://registry.color.org/rgb-registry/srgb). The result rounds to `#ff3900`.

This preserves dominant hue while reducing saturation to fit sRGB. It is not a monochromatic light source or a measured calibration of a particular display. HDR settings, calibration, and ambient light affect appearance.

## Compatibility

Supported: stable Omarchy 4.x releases with semantic palettes and shell section overrides. Last tested: 2026-10-20 on Omarchy 4.0.6-1; other versions in the range have not been individually tested.

Verified in an isolated omabox desktop with Omarchy 4.0.6-1 and Hyprland 0.56.2. The preview is a genuine 1920 × 1080 SDR screenshot showing Foot, Neovim, and the optional `ric.dd8c` speaker widget with fictional fixture data. The widget is not bundled or required.

Omarchy generates app configurations from `colors.toml`. Shell text is set independently through `shell.bar.toml`; selected controls and focus styling use `shell.controls.toml`. Icon theme: `Yaru-wartybrown-dark`. No install scripts.
