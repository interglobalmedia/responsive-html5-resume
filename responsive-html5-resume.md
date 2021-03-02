<h1 class="capitalize">COMD2451</h1>
<h2 class="capitalize center">How to create a responsive HTML5 Resume</h2>

---

<section class="section">
	<h2 class="sentence">Inspiration for the Résumé Page</h2>

I ***found*** a ***very nice*** `responsive HTML5 résumé` on `Codepen` that I ***think*** will be a ***great structure*** and ***design*** to `emulate` in our `portfolio site`. I am **making** *SOME* **modifications** that will ***make*** the `resume` ***more semantic***, but I ***love*** the ***look***.
To ***view*** this `resume` on `Codepen`, please ***visit*** [HTML5 Resume: Jared Pearce](https://codepen.io/jaredpearce/pen/iBdxb) on `Codepen`.

</section>

---

<section class="section">
	<h2 class="sentence">Creating The HTML5 Skeleton</h2>

The ***first thing*** we ***have*** to ***do*** before ***anything else***, is to ***create*** our `HTML5 skeleton` with the `Brackets HTML Skeleton` ***extension***.

**Reminder**: Since I found out that `Adobe Brackets` has been ***deprecated***, I have ***switched over*** to [Atom[(https://atom.io/)], because it has **much** of the ***same feel*** as `Adobe Brackets` did. I thought maybe you would like to **keep** that "feel" ***with you***. I am making a `slide deck` ***related*** to to `Atom` (saving new files and folders follow the same process in `Atom`, so you can still refer to the [Installing and Setting up Brackets
](https://github.com/interglobalmedia/brackets-installation-setup/blob/master/brackets-installation-setup.md) `slide deck`. If, however, you have ***opted*** for `VS Code`, that is fine too!

***Under*** `Elements`, ***inside*** the `HTML5 Skeleton` ***modal***, ***select*** `Basic HTML Skeleton` and `External Stylesheet`. Then ***click*** `Done`.

***Next***, make sure to ***fill in*** the ***value*** of the `html element`'s `lang` ***attribute*** with `en` ***inside*** the ***empty*** `double quotes` which is ***located*** in the `opening tag` of the `html element`.

***Next***, make sure to ***add*** `content` to the `title element` ***inside*** the `head` of the `HTML document`. I for ***instance***, would do the ***following***:

```html
<title>Maria D. Campbell's Responsive HTML5 Developer Resumé</title>
```

***Next***, we `have` to ***move*** the ***inserted*** `link element` which will ***point*** to our `external stylesheet` into the `head` of the `HTML document`, and ***place it*** `under` the `title element`.

</section>

---

<section class="section">
	<h2 class="sentence">Creating the Intro Section of the Résumé</h2>

I am **assuming** that you have ***already created***

+ your `HTML skeleton`, which should ***include*** your `<!DOCTYPE html>` declaration,

+ ***followed by*** an `opening HTML tag` **containing** the `lang attribute` **with** the `value` of `"en"`,

+ then your `head element` which **should contain** a `meta charset element`, a `meta viewport element`, a `title element`, and an `external resource link element` **containing** the `path` to your **external** `CSS` **file**,

+ an **opening** and **closing** `body tag`

The ***first thing*** we ***have*** to ***do*** is to ***create*** an ***introduction area*** at the ***top*** of the `resume`, ***describing*** a **bit** about ***ourselves***. ***Before*** we ***do that***, ***however***, we ***add*** the `main element`, which will ***wrap around*** the ***whole content*** of the `resume`. ***Something*** like ***this***:

```html5
<body>
	<main class="main">

	</main>
</body>
```

I ***also added*** a `class` called `"main"` to the `opening tag` of the `main element`.

***Next***, we can ***add*** a `section element` with an `"introduction"` ***class*** where our `resume introduction` will ***reside***:

```html5
<body>
	<main class="main">
		<section class="introduction">
		</section>
	</main>
</body>
```

***Next***, ***inside*** the `section element` ***with*** the `class` of `"introduction"`, we can ***add*** `something like` the ***following***:

```html5
<section class="introduction">
	<!--1. Header -->
	<header>
		<h1>Maria D. Campbell</h1>
		<h2>Full Stack Developer</h2>
		<p>Full Stack Developer who is passionate about designing,
			developing, and teaching
			experiences that make people's lives simpler.</p>
	</header>
</section>
```

</section>

---

<section class="section">
	<h2 class="sentence center">Bonus: Must-Have Atom Extensions</h2>
	<h3 class="sentence center">Similar to Adobe Brackets</h3>
</section>

---

<section class="section">
	<h2 class="sentence">Must-Have Atom extensions</h2>

+ `atom-beautify`: Beautify HTML, CSS, JavaScript, PHP, Python, Ruby, Java, C, C++, C#, Objective-C, CoffeeScript, TypeScript, Coldfusion, SQL, and more in Atom.

+ `atom-css-comb`: CSScomb is a coding style formatter for CSS (LESS|SASS|SCSS). You can easily write your own configuration to make your style sheets beautiful and consistent.

+ `atom-live-server`: Launch a http server with live reload capability.

+ `color-picker`: Right click and select Color Picker, or hit CMD-SHIFT-C/CTRL-ALT-C to open it. Currently reads HEX, HEXa, RGB, RGBa, HSL, HSLa, HSV, HSVa, VEC3 and VEC4 colors – and is able to convert between the formats.

It also inspects Sass and LESS color variables. Just open the Color Picker with the cursor at a variable and it'll look up the definition for you. From there, you can click the definition and go directly to where it's defined.

+ `css-grid-snippets`: CSS Grid Layout Snippets.

+ `css-snippets`: CSS, SCSS, Sass, and Less Snippets.

+ `html-tag-auto-complete`: A simple auto completion of html tags with class and/or id.

+ `html-template-generator`: HTML template generator for Atom text editor. *

+ `html-to-css`: Generate CSS classes from HTML structure.

+ `ide-css`: Atom-IDE for CSS, LESS and SCSS language.

+ `ide-html`: Atom-IDE for HTML, Go Template, Mustache and other Templates.

+ `linter`: Linter is a base linter provider for the hackable Atom Editor. Additionally, you need to install a specific linter for your language. You will find a full list on [atomlinter.github.io](https://atomlinter.github.io/).

It provides a top-level API to its consumer so that they can visualize errors and other types of messages with ease.

+ `linter-csslint`: Lint CSS on the fly, using csslint. It will be used with files that have the "CSS" or "HTML" syntax.

+ `linter-spell`: Multilingual grammar-specific spell checking using Ispell-interface such as Aspell or Hunspell..

+ `linter-ui-default`: Default UI for the Linter package.

+ `platformio-ide-terminal`: A terminal package for Atom, complete with themes, API and more for PlatformIO IDE. Fork of terminal-plus.

</section>

---

<section class="section">
	<h2 class="sentence">Related Resources</h2>

+ [CSS element+element Selector: w3schools](https://www.w3schools.com/cssref/sel_element_pluss.asp)
</section>

---
