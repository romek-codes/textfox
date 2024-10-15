# textfox

_a port of spotify tui to firefox_

> [!NOTE]
> I am very shocked at how big this got so quickly, I would say that the project
> is still a bit immature, but progress i being made, I welcome PR's from anyone
> wanting to contribute.

## preview

![image](https://github.com/adriankarlen/textfox/blob/main/misc/preview.png)

## Prequisites

- Sidebery

## Installation

1. Download the files
2. Go to `about:profiles`
3. Find your profile -- ( _„This is the profile in use and it cannot be deleted.”_ )
4. Open the profile's root directory
5. Move the files chrome directory and user.js there
6. Restart firefox

> [!NOTE]
> If you don't want to use the provided user.js, please read through it and
> apply the settings in `about:config` manually. These are needed for the css to
> work.

### Sidebery

Sidebery css is being set from within `content/sidebery` (applied as content to
the sidebery url). If you have any prexisting css set from within the sidebery
settings, they might clash or make it so that the sidebery style does not match
the example.

#### Settings

The theme was made using a reset sidebery config, so there should not be
anything crazy needed here, notable settings being set is using the **plain**
theme and **firefox** color scheme. If you want to you can import the sidebery
settings provided.

> [!IMPORTANT]
> **Importing sidebery settings overwrites your current settings, do this at
> your own risk.**

## Customization

The icon configuration utilizes code that is originally from ShyFox, therefore
the same settings are used (these can be set in about:config).
| Setting | true | false (default) |
| -------------------------------------- | --------------------------------------------------------------------- | ------------------------- |
| `shyfox.enable.ext.mono.toolbar.icons` | Supported extensions get monochrome icons as toolbar buttons | Standard icons used |
| `shyfox.enable.ext.mono.context.icons` | Supported extensions get monochrome icons as context menu items | Standard icons used |
| `shyfox.enable.context.menu.icons` | Many context menu items get icons | No icons in context menus |

### CSS configurations
Inside `variables.css` reused variables are stored at the top, tweak those to
your liking without any fear of breaking stuff.

### Acknowledgements

[Naezr](https://github.com/Naezr) - Icon logic and some sideberry logic.

изз - starting working on a similar project in the glazewm discord, prompted me
to get started on the work.
