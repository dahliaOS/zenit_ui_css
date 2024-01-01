<p align="center">
<a href="https://dahliaos.io">Website</a> •
<a href="https://dahliaos.io/discord">Discord</a> •
<a href="https://dahliaos.io/download">Releases</a> •
<a href="https://dahliaos.io/donate">Donate</a> •
<a href="https://docs.dahliaos.io">Documentation</a>


<div>
  <h1 align="center">ZenitUI CSS</h1>
  <p align="center">
  Design beautiful web apps using CSS.
  </p>
</div>

### What is ZenitUI CSS?

ZenitUI CSS is a CSS framework that helps you design beautiful web apps using CSS.

Unlike almost any other CSS framework, ZenitUI CSS provides css only components where possible. This means that you don't have to use JavaScript for every component.

![image](https://github.com/dahliaOS/zenit_ui_css/assets/58103738/aab733e0-9193-44e7-8a22-b32507fcdbd3)

### Contributing

If you feel like something is missing or could be improved, don't hesitate to open a pull request or an issue.

### Content:
- [Installation](#installation)
- [Features](#features)
    - [Accent Colors](#accent-colors)
    - [Dark and Light Mode Support](#dark-and-light-mode-support)
    - [Fonts and Icons](#fonts-and-icons)
    - [Light or dark mode only classes](#light-or-dark-mode-only-classes)
- [Components](#components)
    - [Buttons](#buttons)
    - [Inputs](#inputs)
    - [Select](#select)
    - [Radio](#radio)
    - [Toggle](#toggle)
    - [Card](#card)
    - [List](#list)
    - [Tabs](#tabs)
    - [Carousel](#carousel)

### Installation
Add this line to your HTML file:
```html
<link rel="stylesheet" href="https://cdn.statically.io/gh/dahliaOS/zenit_ui_css/main/zenitUI.css">
```

### Features

ZenitUI CSS comes with a lot of features. Here are some of them:

#### Accent Colors

ZenitUI CSS supports accent colors. You can change the accent color by adding this line to your HTML file:

Note that this line is optional. If you don't add this line, the accent color will be set to the default color (Sky Blue).

```html
<style>:root {--accent-color: var(--blood_red);}</style>
```

ZenitUI CSS comes with the following accent colors:

```css
    /* Aqua Blue */
    --aqua_blue_light: rgb(0, 153, 247);
    --aqua_blue_dark: rgb(0, 123, 217);

    /* Blood Red */
    --blood_red_light: rgb(240, 0, 40);
    --blood_red_dark: rgb(213, 0, 26);

    /* Leaf Green */
    --leaf_green_light: rgb(0, 178, 110);
    --leaf_green_dark: rgb(0, 153, 102);

    /* Magma Orange */
    --magma_orange_light: rgb(255, 77, 0);
    --magma_orange_dark: rgb(229, 80, 0);

    /* Pine Teal */
    --pine_teal_light: rgb(0, 128, 105);
    --pine_teal_dark: rgb(0, 102, 88);

    /* Sky Blue */
    --sky_blue_light: rgb(4, 117, 247);
    --sky_blue_dark: rgb(4, 94, 221);

    /* Dahlia Color Set */
    --dahlia_orange: rgb(255, 61, 0);
```

You can also change the accent color to a custom color by adding this line to your HTML file:

```html
<style>:root {--accent-color: #ff0000;}</style>
```

#### Dark and Light Mode Support

ZenitUI CSS supports dark and light mode. It also provides a button to toggle between dark, system and light mode.

To add the theme toggle button to your HTML file, add this line:

```html
<div class="zenit_theme_toggle">
    <input type="radio" name="options" id="toggle_system">
    <input type="radio" name="options" id="toggle_light" checked>
    <input type="radio" name="options" id="toggle_dark">
    <label for="toggle_dark"><i class="material-icons">dark_mode</i></label>
    <label for="toggle_light"><i class="material-icons">light_mode</i></label>
    <label for="toggle_system"><i class="material-icons">devices</i></label>
</div>
```

#### Fonts and Icons

ZenitUI CSS uses the Manrope font by default. It also comes with material icons.

Here is an example of how to use a material icon in a button:

```html
<button class="icon"><i class="material-icons">add</i></button>
```

#### Light or dark mode only classes

Similar to Github md files, you can use the following classes to make an element visible only in light or dark mode:

```html
<p class="light_mode_only">This text is only visible in light mode.</p>
<p class="dark_mode_only">This text is only visible in dark mode.</p>
```

### Components

#### Buttons

Primary Button:

```html
<button class="primary bg_sky_blue">Primary</button>
```

Secondary Button:

```html
<button class="secondary">Secondary</button>
```

Disabled Button:

```html
<button disabled>Disabled</button>

Pill shaped button:

```html
<button class="pill">Pill</button>
```

Icon Button with text:

```html
<button class="icon-text"><i class="material-icons">cloud</i>Cloud</button>
```

Icon Button:

```html
<button class="icon"><i class="material-icons">cloud</i></button>
```

#### Inputs

Text Input:

```html
<input type="text" class="input" placeholder="Enter your Email address here"></input>
```

With autofocus:

```html
<input type="text" class="input" placeholder="Enter your Email address here" autofocus></input>
```

Disabled:

```html
<input type="text" class="input" placeholder="Enter your Email address here" disabled></input>
```

#### Select

```html
<select>
    <option>Select</option>
    <option>zenitUI CSS</option>
</select>
```

disabled:

```html
<select disabled>
    <option>Select</option>
    <option>zenitUI CSS</option>
</select>

#### Checkbox

```html
<input type="checkbox">
```

checked:

```html
<input type="checkbox" checked>
```

#### Radio

```html
<input type="radio">
```

checked:

```html
<input type="radio" checked>
```

#### Toggle

```html
<input type="checkbox" class="toggle" id="toggle" /><label class="toggle" for="toggle"></label>
```

checked:

```html
<input type="checkbox" class="toggle" id="toggle1" checked/><label class="toggle" for="toggle1"></label>
```

#### Card

```html
<div class="card">
    <p>Card</p>
</div>
```

#### List

```html
<div class="list">
    <p>1</p>
    <p>2</p>
    <p>3</p>
</div>
```

#### Tabs

```html
<div class="tabs">
	<input type="radio" name="tabs" id="tab1" checked>
    <label for="tab1"><i class="material-icons">spa</i> Tab 1</label>
	<div>Tab with text and icon</div>
	<input type="radio" name="tabs" id="tab2">
    <label for="tab2">Tab 2</label>
	<div>Tab with text only</div>
    <input type="radio" name="tabs" id="tab3">
    <label for="tab3"><i class="material-icons">spa</i></label>
    <div>Tab with icon only</div>
</div>
```

#### Carousel

```html
<ul class="zenit_carousel">
    <li>1</li>
    <li>2</li>
    <li>3</li>
    <li>4</li>
    <li>5</li>
    <li>6</li>
</ul>
```

## License

<p align="left">
  <img width="30%" src="https://github.com/dahliaOS/brand/blob/main/dahliaOS/logotype/svg/logotype-dark.svg#gh-dark-mode-only"/>
  <img width="30%" src="https://github.com/dahliaOS/brand/blob/main/dahliaOS/logotype/svg/logotype-light.svg#gh-light-mode-only"/>
</p>

Copyright @ 2019-2024 - The dahliaOS Authors - contact@dahliaos.io

This project is licensed under the [Apache 2.0 license](/LICENSE)
