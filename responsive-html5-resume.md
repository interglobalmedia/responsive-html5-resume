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

**Reminder**: Since I found out that `Adobe Brackets` has been ***deprecated***, I have ***switched over*** to [Atom](https://atom.io/), because it has **much** of the ***same feel*** as `Adobe Brackets` did. I thought maybe you would like to **keep** that "feel" ***with you***.

I have created a slide deck called [Atom Installation and Setup](https://github.com/interglobalmedia/atom-installation-setup/blob/master/atom-installation-setup.md) slide deck which I **hosted** on `Github`. There, I include `extensions` you should ***add*** to `Atom`. **Saving** new `files` and `folders` ***follow*** the `same process` in `Atom`, so you can ***still refer*** to the [Installing and Setting up Brackets
](https://github.com/interglobalmedia/brackets-installation-setup/blob/master/brackets-installation-setup.md) `slide deck`. If, ***however***, you have ***opted*** for `VS Code`, that is fine too!

***Under*** `Elements`, ***inside*** the `HTML5 Skeleton` ***modal***, ***select*** `Basic HTML Skeleton` and `External Stylesheet`. Then ***click*** `Done`.

***Next***, make sure to ***fill in*** the ***value*** of the `html element`'s `lang` ***attribute*** with `"en"` ***inside*** the ***empty*** `double quotes` (`""`) which is ***located*** in the `opening tag` of the `html element`. If you have ***opted*** for `Atom`, it will just be a ***matter*** of **deleting** `HTML markup` that you ***don't initially*** **need**. To **create** an `HTML`(5) `Skeleton` with `Atom`, ***select*** the `Atom` **menu tab** called `Packages`, then ***select*** `HTML Template Generator`, and then `generate HTML Template`. An `HTML Template Generator popup` will **appear**:

<div>
	<img src="images/atom-html-template-generator.png" alt="Atom HTML Template Generator">
</div>

Simply ***click*** the `"Generate"` **button**, and it will **create** an `HTML "template"` for you in your **current active** `HTML` **file**.

***Next***, make sure to ***add*** `content` to the `title element` ***inside*** the `head` of the `HTML document`. I for ***instance***, would do the ***following***:

```html
<title>Maria D. Campbell's Responsive HTML5 Developer Resumé</title>
```

***Next***, we `have` to ***move*** the ***inserted*** `link element` which will ***point*** to our `external stylesheet` into the `head` of the `HTML document`, and ***place it*** `under` the `title element`.

The ***cool thing*** about `Atom` is that it will **include** the `dir` **attribute** with a `value` of `"ltr"` **inside** the `opening tag` of the `html element`. So if any of you are ***into*** `Writing Modes`, you **might want** to **use** `Atom`!

</section>

---

<section class="section">
	<h2 class="sentence">Creating the Intro Section of the Résumé</h2>

I am **assuming** that you have ***already created***

+ your `HTML skeleton`, which should ***include*** your `<!DOCTYPE html>` declaration,

+ ***followed by*** an `opening HTML tag` **containing** the `lang attribute` **with** the `value` of `"en"`,

+ then your `head element` which **should contain** a `meta charset element`, a `meta viewport element`, a `title element`, and an `external resource link element` **containing** the `path` to your **external** `CSS` **file**,

+ an **opening** and **closing** `body tag`

So **right now** your `resume.html` **page** should look **something like** the ***following***:

```html5
<!DOCTYPE html>
<html lang="en"
	  dir="ltr">

<head>
	<meta charset="utf-8">
	<meta name="viewport"
		  content="width=device-width, initial-scale=1.0">
	<meta name="description"
		  content="Maria D. Campbell's Online Portfolio Site, Web Developer and Web Development Teaching Resume">
	<meta name="keywords"
		  content="Babel JavaScript Compiler, CSS, CSS3, CSS Flexbox, Command Line Interface, CSS Grid, Embedded JavaScript (EJS), ECMAScript 6 Plus, ES6 Modules, Express.js, Final Cut Pro, Git, Github, Heroku
, Final Cut Pro, Git. Github, Heroku, HTML5, JetBrains, Jira, Modern JavaScript, MongoDB, Netlify, Netlify CMS, Node.js, NPM, PostreSQL, Python 3.8+, React, SASS (SCSS), Webpack, WordPress">
	<meta name="
		  Author"
		  content="Maria D. Campbell">
	<title>Maria Campbell's Online Résumé</title>
	<link rel="stylesheet"
		  href="styles/resume.css">
</head>

<body>

</body>
</html>
```

If you are **using** `Atom` and **something like** a `div element` has been **added** between the `opening` and `closing body tags`, **remove it**. We don't need it. It is a ***completely*** `un-semantic element` that should be ***avoided***. There is a **time** and **place** for it, but ***not here***.

The ***first thing*** we ***have*** to ***do*** is to ***create*** an ***introduction area*** at the ***top*** of the `resume`, ***describing*** a **bit** about ***ourselves***. ***Before*** we ***do that***, ***however***, we ***add*** the `main element`, which will ***wrap around*** the ***whole content*** of the `resume`. ***Something*** like ***this***:

```html5
<body>
	<main role="main">

	</main>
</body>
```

I ***also added*** a `role attribute` with the value of `"main"` to the `opening tag` of the `main element`. This `attribute` with the `value` of `"main"` **indicates** that the `main element` ***contains*** the `main content` of the **page**.

***Next***, we can ***add*** a `div element` with a `"page"` ***class*** which acts as a `wrapper` **around** our **content**, and **where** we will ***add styling*** that will make our `resume` look like an ***actual*** `page/piece` of `paper`.

```html5
<body>
	<main class="main">
		<div class="page">
		</div>
	</main>
</body>
```

I am ***not concerned*** about whether or not the `div element` is **semantic**. It is added ***solely*** for `styling purposes`.

***Next***, ***inside*** the `div element` ***with*** the `class` of `"page"`, we can ***add*** `something like` the ***following***:

```html5
<body>
<main class="main">
	<div class="page">
		<header>
			<h1>Maria D. Campbell</h1>
			<h2>Full Stack Developer</h2>
			<p>Full Stack Developer who is passionate about designing,
				developing, and teaching
				experiences that make people's lives simpler. Specialty
				is to help sharpen the thinking of individuals
				in approaching their workflows in a more organized and
				efficient manner, thereby preparing them for jobs in Web
				Design and Development.</p>
		</header>
		</div>
	</main>
</body>
```

</section>

---

<section class='section"'>
	<h2 class="sentence"></h2>
</section>

---

<section class="section">
	<h2 class="sentence">Related Resources</h2>

+ [CSS element+element Selector: w3schools](https://www.w3schools.com/cssref/sel_element_pluss.asp)

+ [RoleAttribute: Wikipedia](https://www.w3.org/WAI/PF/HTML/wiki/RoleAttribute)

+ [What is WAI-ARIA, what does it do for me, and what not?](https://www.marcozehe.de/what-is-wai-aria-what-does-it-do-for-me-and-what-not/)
</section>

---
