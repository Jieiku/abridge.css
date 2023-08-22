<div align="center">
<img src="https://raw.githubusercontent.com/Jieiku/abridge.css/master/abridge.svg"/>

# Abridge CSS

Abridge.css is a CSS library for semantic html, it adds a nice default style for all HTML elements. This was originally created to be used as a classless or optionally class-light framework for a semantic html Zola Blog Theme. It can save you a lot of time when you need to style HTML for your HTML/React/Vue demo on CodePen/CodeSandbox. It can also be used as a base style for your blog/website.

Maintainence of this project is made possible by all the <a href="https://github.com/Jieiku/abridge.css/graphs/contributors">contributors</a> and <a href="https://github.com/sponsors/Jieiku">sponsors</a>. If you'd like to sponsor this project and have your avatar or company logo appear below <a href="https://github.com/sponsors/Jieiku">click here</a>. 💖

<!-- sponsors --><!-- sponsors -->

---

**[View demo](https://abridgecss.netlify.app/)**

</div>

Abridge CSS uses [normalize.css](https://github.com/necolas/normalize.css/) and [sanitize.css](https://github.com/csstools/sanitize.css) to ensure consistent styling across browsers (no IE support). When using Abridge CSS, you don't need to include `normalize.css` or `sanitize.css` anymore.

Abridge CSS uses CSS variables and is structured to be modular, so you can include only the parts that you need. There are three themes included: light, dark, and automatic. The automatic theme will display either a light or dark theme depending on the users browser preference setting. (prefers-color-scheme: dark)

Abridge CSS is very lightweight, and the size can be further tuned by including only what you plan to use.

I created Abridge.css primarily to use with Zola, and because I was after a set of features: semantic/classless, dark mode, responsive text, Normalize, Sanitize, and overall small size. I researched various css frameworks prior to creating this framework: [tabulated comparison of css frameworks](https://github.com/Jieiku/classless-css/blob/master/README.md)

## Features:

- Drop in to use, no configuration.
- Class-light (there are very few classes)
- Consistent styling across browsers thanks to `normalize.css` and `sanitize.css`
- Responsive
- Supports light and dark themes (automatically detect the OS/browser mode and switch)
- Uses CSS variables
- Uses `rem`
- Lightweight
- Semantic

## Download

See [https://raw.githubusercontent.com/Jieiku/abridge.css/master/dist/abridge.css](https://raw.githubusercontent.com/Jieiku/abridge.css/master/dist/abridge.css)

## Customizing

Abridge SASS variables can be overrided by editing `sass\abridge.scss` file in your project's root sass folder.

### Page Width:

```scss
$mw:75%,// max-width
```

### Abridge Theme Modes

```scss
$abridgeMode: "switcher",//valid values: switcher, auto, dark, light
```

- Switcher automatically displays a dark or light version depending on browser/OS settings, and has a javascript user clickable theme switcher.
- Auto automatically displays a dark or light version depending on browser/OS settings.
- Dark is the dark theme always.
- Light is the light theme always.

### Colors and Styles

You can specify which color template you want to use as a base:
```scss
$color: "orange",// color template to use/override: orange, blue, blueshade
```

Then override individual colors as needed:
```scss
/// Dark Colors
$f1d: #ccc,// Font Color Primary
$f2d: #ddd,// Font Color Headers
$c1d: #111,// Background Color Primary
$c2d: #222,// Background Color Secondary
...
```

## Compiling:

install nodejs: https://nodejs.org/

```bash
git clone https://github.com/Jieiku/abridge.css
cd abridge.css
npm install sass
npm run-script main
```

## Credits
- [new.css](https://github.com/xz/new.css)
- [bamboo.css](https://github.com/rilwis/bamboo)
- [pico.css](https://github.com/picocss/pico)
- [Basic.css](https://github.com/vladocar/Basic.css)
- [AttriCSS](https://github.com/raj457036/attriCSS)
- [normalize.css](https://github.com/necolas/normalize.css)
- [sanitize.css](https://github.com/csstools/sanitize.css)
- [Feather Icons](https://github.com/feathericons/feather)
- [Tabler Icons](https://github.com/tabler/tabler-icons)
