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
		<h1><a href="index.html">Maria D. Campbell</a></h1>
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

I **add** an `a element` to the `h1` ***inside*** the `header element` so that a **user** can `click` on it to **easily** and **quickly** ***return*** to the `home page` (`index.html`) **instead of** having to **scroll** all the way **down** to the ***bottom*** of the `page`. However, there is a `footer navigation` available there that **links** to **all** the **pages** on the `site` as well.

</section>

---

<section class="section">
	<h2 class="sentence">The Professional Experience Section</h2>

**Next**, **below** the `closing header tag`, I **add** an `opening section tag` with the **class** of `"professional_experience"`. Then I **create** a `closing section tag`. Then, **making sure** that the `cursor` is ***placed between*** the `opening` and `closing section tags`, I **press** the `return key` to **take** the `closing section tag` to the **next line**.

**Below** the `opening section tag` with the **class** of ``"professional_experience"``, I **add** an `opening article tag`. Then I **create** a `closing article tag`. Then, **making sure** that the `cursor` is **placed between** the `opening` and `closing article tags`, I **press** the `return key` to **take** the `closing article tag` to the **next line**.

**Below** the `opening article tag`, I **add** an `h2 element` with the `text content` of `"Professional Experience"`.

***Right now*** the `section element` with the **class** of `"professional_experience"`, the `article element` **containing** the `h2 element` with the `text content` of `"Professional Experience"` should **look** like **this**:

```html5
<section class="professional_experience">
	<article>
		<h2>Professional Experience</h2>
	</article>
</section>
```

</section>

---

<section class="section">
	<h2 class="sentence">Adding the first section with an h3 heading</h2>

**Next**, **below** the `h2 heading` within the `article element` **containing** the `text content` of `"Professional Experience"`, I **add** an `opening section tag`. Then I **create** a `closing section tag`. Then, **making sure** that the `cursor` is **placed between** the `opening` and `closing section tags`, I **take** the `closing section tag` to the **next line**.

**Below** the `opening section tag`, I **add** an `h3 element`, **including** both the `opening` and `closing h3 tags`. Then, **making sure** that the `cursor` is **placed between** the `opening` and `closing h3 tags`, I **press** the `return key` and **take** the `closing h3 tag` to the **next line**.

**Right now** the `Professional Experience "section"` of the `resume.html` should **look like** the **following**:

```html5
<section class="professional_experience">
	<article>
		<h2>Professional
			Experience</h2>
		<section>
			<h3>
			</h3>
		</section>
	</article>
</section>
```

**Next**, **between** the `opening` and `closing h3 tags` **inside** the `section element` **inside** the `article element`, I **add** the **following content**:

```html5
<h3>Adjunct Professor <span class="time"><time
			  datetime="2020-01-29"
			  class="start">2020</time>
		&#8211; Present</span>
</h3>
```

There is ***a lot*** `going on` over here that is ***new***, so let's `break it down` a bit.

+ The **text content** `"Adjunct Professor"` that **follows** the `opening h3 tag` is my `title`. That is ***also where*** you would **place** the `title` of your ***most current*** `job/position`.

+ The `span element` with the **class** of `"time"` is **meant** to **be able** to **change** the `color` of the `text` **within** the `span element`, thereby **differentiating** it **from** the `text content` **between** the `opening` and `closing time tags`. This is ***purely*** for **design purposes**. Like the `div element`, the `span element` has ***absolutely no semantic value***. In other words, **no meaning** to the `browser` or `search engines` (`SEO`).

+ I **use** the `time element` for **semantic reasons**. The [time element](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/time) **represents** a **specific period** in **time**. It ***may include*** the `datetime` **attribute** to **translate dates** into `machine-readable format`, **allowing** for **better search engine results** or **custom features** such as **reminders**.

`datetime`: the `datetime attribute` of the `time element` **indicates** the `time` and/or `date` of the `element` and ***must be*** in **one** of the **following formats** (`valid datetime values`):

+ `valid year string`: "2011", i.e.

+ `valid month string`: "2011-11", i.e.

+ `valid yearless date string`: "11-18", i.e.

+ `valid week string`: "2011-W47", i.e.

+ `valid time string`: "14:54", "14:54:39", or "14:54:39.929", i.e. (24 hour clock aka military time)

+ `valid local date and time string`: "2011-11-18T14:54:39.929", "2011-11-18 14:54:39.929", i.e.

+ `valid global date and time string`: "2011-11-18T14:54:39.929Z", "2011-11-18T14:54:39.929-0400", "2011-11-18T14:54:39.929-04:00", "2011-11-18 14:54:39.929Z", "2011-11-18 14:54:39.929-0400
", "2011-11-18 14:54:39.929-04:00", i.e.

+ `valid duration string`: "PT4H18M3S", i.e.

I **am using** the `valid date string`: `datetime="2020-01-29"`. I ***don't use*** it for `"Present"`, because that is ***not*** an `end time`. I **give** the `time element` the **class** of `"start"` because it **represents** the `start time` for this **particular position**.

`&#8211;` is the [html symbol entity](https://www.w3schools.com/html/html_symbols.asp) for `-`.

+ I **only add** the `text content` of `2020` because the **time element** is **providing** the ***specifics*** to the `browser` and `search engines`, and I **want** to have **enough space** to ``"print"`` the `start date`, the `dash`, and the `text content` of `"Present"` to the **page**. This is ***more*** of a **style decision**, **taking** into **account** that the `time element` will do the ***informational*** **heavy lifting** for me!

</section>

---

<section class="section">
	<h2 class="sentence">Adding the first p element to the first Professional Experience section element</h2>

**Below** the `closing h3 tag` which **contains** the `position title`, I **add** a `p element` (`opening` and `closing tags`). **Between** the `opening` and `closing p tags`, I **add** the **following** `text content`:

```html5
<p><strong>
		New York City College
		of
		Technology</strong>
	<b>Brooklyn,
		N.Y.</b>
</p>
```

As seen above, **right after** the `opening p tag`, I **add** a `strong element`. This is **meant** for ***emphasis***, because the **employer** of the **position** is of `high importance`. **Between** the `opening` and `closing strong tags`, I **add** my **employer**. In ***this case***, the `text content` is `"New York City College of Technology"`.

**After** the `closing strong tag`, I **add** a `b element`. This ***indicates*** that the `text content` **between** the `opening` and` closing b tags` is ***not*** as **important** as the `text content` **between** the `opening` and `closing strong tags`. The `text content` of the `b element` ***represents*** the **location** of the **employer**.

The `closing b tag` is **followed by** the `closing p tag`.

**Right now**, `Professional Experience` should **look like** the **following**:

```html5
<section class="professional_experience">
	<article>
		<h2>Professional
			Experience</h2>
		<section>
			<h3>Adjunct Professor <span class="time"><time
						  datetime="2020-01-29"
						  class="start">2020</time>
					&#8211; Present</span>
			</h3>
			<p><strong>
					New York City College
					of
					Technology</strong>
				<b>Brooklyn,
					N.Y.</b>
			</p>
		</section>
	</article>
</section>
```

</section>

---

<section class="section">
	<h2 class="sentence">Adding a second p element below the first</h2>

**Next**, I **add** a **second** `p element` of which the `text content` **further describes** the **targeted position**. Mine **looks like** the **following**:

```html5
<p><strong>Communication Design</strong></p>
```

**This** `text content` ***states*** that the **position** is **within** `Communication Design` (`department`) at the **College**.

**Now** the `Professional Experience` **section** of the `resume.html` **page** should **look like** the **following**:

```html5
<section class="professional_experience">
	<article>
		<h2>Professional
			Experience</h2>
		<section>
			<h3>Adjunct Professor <span class="time"><time
						  datetime="2020-01-29"
						  class="start">2020</time>
					&#8211; Present</span>
			</h3>
			<p><strong>
					New York City College
					of
					Technology</strong>
				<b>Brooklyn,
					N.Y.</b>
			</p>
			<p><strong>Communication Design</strong></p>
		</section>
	</article>
</section>
```

</section>

---

<section class="section">
	<h2 class="sentence">Adding a ul element to the position title section</h2>

**Next**, **below** the ***second*** `p element` with the **content** of `<strong>New York City College of Technology</strong> <b>Brooklyn, N.Y.</b>`, I **add** an `opening ul tag`. **Inside** the `opening ul tag`, I **add** the **class** of `"position-points"`. Then I **add** a `closing ul tag`. The `closing ul tag` is located **right above** the `closing section tag` for ***that*** `position section`. Then, **making sure** that the `cursor` is **between** the `opening` and `closing ul tags`, I **press** the `return key` and **take** the `closing ul tag` to the **next line**.

**Next**, **below** the `opening ul tag`, I **add** 4 `li elements`, because I **want** to **add** 4 `position points` **regarding** the `position`. That is ***why*** I **added** the **class** of `"position-points"` to the `opening ul tag`. It **describes** the **purpose** of the `unordered list`.

**Now**, the `"Professional Experience"` **section** should **look like** the **following**:

```html5
<section class="professional_experience">
	<article>
		<h2>Professional
			Experience</h2>
		<section>
			<h3>Adjunct Professor <span class="time"><time
						  datetime="2020-01-29"
						  class="start">2020</time>
					&#8211; Present</span>
			</h3>
			<p><strong>
					New York City College
					of
					Technology</strong>
				<b>Brooklyn,
					N.Y.</b>
			</p>
			<p><strong>Communication Design</strong></p>
			<ul class="position-points">
				<li>Teaching COMD2451 Web Design 1 Spring 2021
					Semester Online. Tools used are Blackboard
					Ultra for video recording/screensharing,
					Google Meet for screenshare meetings on the
					fly, and the Discord app for communication
					between classes. Course content including
					slide decks and homework assignments hosted
					on Github. Students are added as
					collaborators to a private course repository
					on Github. Slide decks created with the
					reveal.js markdown version (reveal-md npm
					package) for quicker completion of the
					decks.</li>
				<li>Teaching COMD3663 Dynamic Web 1 in Spring
					Semesters. Focuses on Modern JavaScript,
					mostly on the frontend, and wraps up with
					creating an API application with a
					Node.js/Express.js backend server deployed
					to Heroku.</li>
				<li>Seamlessly transitioned the class from
					on-site learning to remote learning due to
					the COVID-19 pandemic using tools such as
					Discord, Black Board Ultra, and Github.</li>
				<li>Students could contact fellow students and
					share information related to
					JavaScript/course on Discord, and I did the
					same. I believe it important to be able to
					maintain continuous communication with my
					students.</li>
			</ul>
		</section>
	</article>
</section>
```

</section>

---

<section class="section">
	<h2 class="sentence">Repeating the position section as many times as necessary</h2>

***For me***, I **repeat** the `"position"` **section** (as **indicated** in the **previous slide**) 5 ***more times***, because I have `five` ***more positions*** I want to **include** in my `résumé`. You **should repeat** the `"position"` **section** as ***many times*** as you **need**. Just **follow** the ***same*** `HTML markup` **structure**, ***including*** any `classes` that have been **added** as well.

</section>

---

<section class="section">
	<h2 class="sentence">Adding div element with the class of "resume_skills" as a wrapper for the aside widgets section</h2>

**Next**, **below** the `closing section tag` of the ***last*** of the `"position"` **section** `closing tags`, I **add** an `opening div tag` with the **class** of `"resume_skills"`. Then I **add** a `closing div tag`. Then, **making sure** that the `cursor` is **placed between** the `opening` and `closing div tags`, I **press** the `return key` and **take** the `closing div tag` to the **next line**. This `closing div tag` **should** be **right above** the `opening footer tag`. I use a `div element` **here**, because I am **not concerned** about `semantic HTMl` for the **purpose** of this `element`. It is ***simply meant*** to **wrap around** the `aside element` which **acts** as a `sidebar` **containing widgets** for `"Sample Work"`, `"Software" skills`, `Education`, in ***my case*** `"Languages"`, `"Achievements"`, and `"Interests"`.

</section>

---

<section class="section">
	<h2 class="sentence">Adding a "sample-work" aside widget</h2>

**Below** the `opening aside tag`, I **add** an `opening section tag` with the **class** of `"sample-work"`. Then I **add** a `closing section tag`, which will be **right above** the ***next*** `opening section tag` with a **class** of `"software"`. Then, **making sure** that the `cursor` is **placed between** the `opening` and `closing section tags`, I **press** the `return key` and **take** the `closing section tag` to the **next line**.

**Below** the `opening section tag` with the **class** of `"sample-work"`, I **add** an `h2 element` with the `text content` of `"Sample Work"`.

**Below** the `h2 element`, I **add** an `opening ul element`. Then I **add** a `closing ul element`. Then, **making sure** that the `cursor` has been **placed between** the `opening` and `closing ul tags`, I **press** the `return key` and **take** the `closing ul tag` to the **next line**.

**Inside** the `ul element`, I **add** 6 `li elements`. **Inside** each `li element`, I **add** an `a` (`anchor`) `element`. **Inside** each of those `a elements`, I **add** an `href attribute` with the `value` of the `absolute path` to the `production site` of the` applications` I **have built** that I ***want*** to `feature` in my `résumé`. **After** the `href attribute` in each of the `a elements`, I **add** the `target attribute` with the `value` of `"_blank"`, **and then** the `rel attribute` with the `value` of ``"noreferrer noopener"``. **After** each `opening a tag`, I **add** the `text content` **describing** the **targeted application** I **want** to **feature**.

This is **how** the `div element` with the **class** of `"resume_skills"` should **look like** at **this point**:

```html5
<div class="resume_skills">
	<aside>
		<section class="sample-work">
			<h2>Sample Work</h2>
			<ul>
				<li><a href="https://pacific-savannah-76659.herokuapp.com/"
					   target="_blank"
					   rel="
					   noreferrer
					   noopener">Chattrbox</a>
				</li>
				<li><a href="https://interglobalmedia.github.io/speech-to-text-app/"
					   target="_blank"
					   rel="
					noreferrer
					noopener">Speech To Text App</a></li>
				<li><a href="https://interglobalmedia.github.io/making-music-in-the-browser/"
					   target="_blank"
					   rel="
					noreferrer
					noopener">Making Music in the
						Browser</a></li>
				<li><a href="https://interglobalmedia.github.io/web-audio-api-ajax/"
					   target="_blank"
					   rel="
					noreferrer
					noopener">Web Audio API and AJAX</a>
				</li>
				<li><a href="https://interglobalmedia-weather-app.herokuapp.com/"
					   target="_blank"
					   rel="
					noreferrer
					noopener">Node.js Server Weather
						App</a>
				</li>
				<li><a href="https://interglobalmedia.github.io/local-storage-session-storage-fun-form/"
					   target="_blank"
					   rel="
					noreferrer
					noopener">Storage Fun with Forms</a>
				</li>
				<!-- <li><a href="https://prod.sandia.gov/wbt/HW100/" target="_blank">Hot Work Training (HW100)</a></li>-->
			</ul>
		</section>
	</aside>
</div>
```

</section>

---

<section class="section">
	<h2 class="sentence">The "software" aside widget</h2>

**Next**, **below** the `closing section tag` for the `"sample-work"` **aside widget**, I **add** an `opening section tag` with the **class** of `"software"`. Then I **add** a `closing section tag`. Then, **making sure** that the `cursor` is **placed between** the `opening` and `closing section tags`, I **press** the `return key` and **take** the `closing section tag` to the **next line**.

**Next**, **right below** the `opening section tag` with the **class** of `"software"`, I **add** an `h2 element` with the `text content` of `"Software"`.

**Next**, **below** the `h2 element` with the `text content` of `"Software"`, I **add** an `opening ul tag` with the **class** of `"technology"`. Then I **add** a `closing ul tag`. Then, **making sure** that the `cursor` is **placed between** the `opening` and `closing ul tags`, I **press** the `return key` and **take** the `closing ul tag` to the **next line**.

**Inside** the `ul element`, I **add** all the `li elements` I **need** to **list** my `software skills`. ***Each*** `li element` **consists of** `two parts`. The `li element` **text content**, and then the `text content` **wrapped inside** a `span element`. The `text content` **directly within** the `li element` **relates to** the `name` of the `software`. The `text content` **within** the `span element` **relates to** the `number` of `years` I have **been using** it. One **such example** is the **following**:

```html5
<li>Babel JavaScript Compiler <span class="exp">6
		years</span></li>
```

I **add** a **class** of `"exp"` **in case** if I **want** to ***style*** that `text content` any **differently** from the ***rest*** of the `text content` **inside** the `li element`. **Here**, it **would be** `"Babel JavaScript Compiler"`.

**However**, the `years using the software` ***does not appear*** on the **page**. I **target** the `span element` with the **class** of `"exp"` **using** the the **property declaration** `display: none;`.

```css
.technology li > span {
	display: none;
}
```

I will be **breaking down** what is **taking place** here ***later on*** when I **go through** the `external stylesheet` for `resume.html`, but I **just wanted** to **point out** that `.technology li > span` is an **example** of a `combinator selector`. **Remember** that ***term*** from the [Basic CSS](https://github.com/interglobalmedia/basic-css/blob/master/basic-css.md) `slide deck`? ***Specifically***, we are **dealing with** a `child combinator selector` here **represented by** the `>` greater than angle bracket.

The `combinator selector` is when ***two*** `simple selectors` are **separated** by a `combinator selector`. When the `simple selectors` are **separated by** a `child selector` (`>`), the `child selector` **selects** `all elements` that are the `children` of a ***specified*** `element`.

The `.technology class` **represents** the `ul element` with the **class** of `.technology`, and the `li > span` **represents** each `li element` **inside** the `ul element`, the `span` **being** the `child` of the `li element`. By **targeting** that **child** `span element` with the **class** of `"exp"` **using** the `property declaration` of `display: none;`, the `text content` **describing** the `number` of `years` ***does not appear*** on the **page**.

I am **doing this** because I **can't use** the `time element` **properly** with `text content` like `"6 years"`. But I **wanted** to **create** `"keywords"` **describing** the `number` of `years` I have **been using** certain `software` for `search engine optimization`, so this is **how** I ***deal*** with it. Even though the `keywords` ***do not appear*** on the **page**, they **still appear** in the `HTML live markup`. You can **check it out** either ***within*** the `Elements tab` in `Chrome Developer Tools`, or ***within*** the `Sources tab` in `Chrome Developer Tools` by **selecting** `index.html` within `Sources`.

**Now** the `aside "software" widget` **section** should ***basically*** look like the **following**:

```html5
<section class="software">
	<h2>Software</h2>
	<ul class="technology">
		<li>Babel JavaScript Compiler <span class="exp">6
				years</span></li>
	</ul>
</section>
```

**Just add** as ***many*** `"software" skills` **using** the `li element` with a **child** `span element` **containing** the **class** of `"exp"` as **many times** as you **need** within the `ul element` with the **class** of `"software"`.

</section>

---

<section class="section">
	<h2 class="sentence">The "education" aside widget</h2>

**Right below** the `closing section tag` for the `"software"` **aside widget**, I **add** an `opening section tag` with the **class** of `"education"`. Then I **create** a `closing section tag`. Then, **making sure** that the `cursor` is **placed between** the `opening` and `closing section tags`, I **press** the `return key` and **take** the `closing section tag` to the **next line**.

**Below** the `opening section tag` with the **class** of `"education"`, I **add** an `h2 element` with the `text content` of `"Education"`.

**Below** the `h2 element` with the `text conten`t of `"Education"`, I **add** an `h3 element` with the `text content` of `"New York Coding and Design Academy"`. This `h3 element` **describes** which school I **have attended**. This `text content` is **followed by** a **self-closing** `<br/> tag`. I **add** the `<br/> tag` so that the `text content` that **follows** goes to the **next line**.

**Below** the `h3 element` with the `text content` of `"New York Coding and Design Academy"`, I **add** a `p element`. Inside the `p element`, I **add** the `text content` and `HTML markup` of:

```html5
<p>Web Development 100 &<br />
	Front-End Development 101
	<b>N.Y., N.Y.</b>
</p>
```

the `text content` **within** the `p element` **describes** which `course`(`s`) I **took** at this ***particular*** `educational institution`. Because I **took more** than **one course** during the ***same period*** of **time**, I **add** the **self-closing** `<br /> element` ***after*** the **name** of the **first course** so that the **name** of the **second course** would ***appear*** on the **next line**.

**Next**, I **wrap** the `location` of **where** I ***took*** the **course** in `opening` and `closing b tags`. Like ***previously***, I **use** the `b element` **instead of** the `strong element` because it is ***not*** important enough to **wrap** in `opening` and `closing strong tags`.

**So far** the `Education` **aside education widget** looks like the **following**:

```html5
<section class="education">
	<h2>Education</h2>
	<h3>New York Coding and Design Academy<br />
		<time datetime="2015-09-15"
			  class="start">9/2015</time>
		<time datetime="2016-02-02"
			  class="end"> &#x2010; 2/2016</time>
	</h3>
	<p>Web Development 100 &<br />
		Front-End Development 101<br />
		<strong>Certificate</strong>
		<b>N.Y., N.Y.</b>
	</p>
</section>
```

I **add** as many `h3 elements` **containing** the **name** of the **school** I ***attended*** along with the `start` and `end dates` **between** the `opening` and `closing h3 tags` **using** the `time element` for the `start date` and ***another*** `time element` for the `end date`. I ***also add*** the **class** of `"start"` to the `time element` **targeting** the `start date`, and a **class** of `"end"` to the `time element` **targeting** the `end date`.

**Below** the `closing h3 tag`, I **add** a `p element` which **contains** the **name**(s) of the **course**(s) I ***took*** and the **location** of the **school**, **making sure** to ***add*** a `<br/> element` **before** the **beginning** of the `text` that I **want** to **take** to the `"next line"`.

**Below** the **names** of the **courses** above, I **add** a `strong element` with the `text content` of `"Certificate"` because that is the `"degree"` I **earned** with the **completion** of the **two courses**. In the **case** of a `College` or `University`, I **add** the **name** of the **degree** I ***earned*** at the **school**. i.e., `"Bachelor of Arts"` or `"Masters"`, **for example**.

My **complete** `"Education" widget` **looks like** the **following**:

```html5
<section class="education">
	<h2>Education</h2>
	<h3>New York Coding and Design Academy<br />
		<time datetime="2015-09-15"
			  class="start">9/2015</time>
		<time datetime="2016-02-02"
			  class="end"> &#x2010; 2/2016</time>
	</h3>
	<p>Web Development 100 &<br />
		Front-End Development 101</br />
		<strong>Certificate</strong>
		<b>N.Y., N.Y.</b>
	</p>
	<h3>New York Coding and Design Academy<br />
		<time datetime="2018-01-15"
			  class="start">1/2018</time><time
			  datetime="2018-06-15"
			  class="end"> &#x2010; 6/2018</time>
	</h3>
	<p>Evening JavaScript Intensive<br />
		<strong>Certificate</strong>
		<b>N.Y., N.Y.</b>
	</p>
	<h3>Columbia University<br />
		School of International and Public Affairs<br />
		<time datetime="2000-05-20"
			  class="end">12/1987</time>
	</h3>
	<p>International Finance
		and Banking<br />Eastern European
		Studies<br /><strong>Masters</strong><b>N.Y.,
			N.Y.</b><br />

	</p>
	<h3>Barnard College<br />
		<time datetime="2000-05-20"
			  class="end">5/1984</time>
	</h3>
	<p>French
		Literature<br />
		<strong>Bachelor
			of Arts</strong> <b>N.Y., N.Y.</b><br />
	</p>
</section>
```

</section>

---

<section class="section">
	<h2 class="sentence">The "languages" aside widget</h2>

**Below** the `closing section tag` for the `"education"` **aside widget**, I **add** an `opening section tag` with the **class** of `"languages"`. Then I **create** a `closing section tag`. Then, **making sure** that the `cursor` is **placed between** the `opening` and `closing section tag`, I **press** the `return key` and **take** the `closing section tag` to the **next line**.

**Below** the `opening section tag` with the **class** of `"languages"`, I **add** an `h2 element` with the `text content` of `"Languages"`.

**Below** the `opening section tag` with the **class** of `"languages"`, I **add** the ***following*** `text content`:

```html5
<p>French • Serbo-Coratian • Learning Spanish</p>
```

If any of you ***speak*** **languages** other than `English`, I think it is **very important** to ***include*** that in your `résumés`. My `"languages"` **aside widget** looks like the **following**:

```html5
section class="languages">
	<h2>Languages</h2>
	<p>French • Serbo-Croatian • Learning Spanish</p>
</section>
```

</section>

---

<section class="section">
	<h2 class="sentence">The "achievements" aside widget</h2>

**Below** the `closing section tag` for the `section element` with the **class** of `"languages"`, I **add** an `opening section tag` with the **class** of `"achievements"`. Then I **create** a `closing section tag`. Then, **making sure** that the `cursor` is **placed between** the `opening` and `closing section tags`, I **press** the `return key` to **take** the `closing section tag` to the **next line**.

**Below** the `opening section tag` with the **class** of `"achievements"`, I **add** an `h2 element` with the `text content` of `"Achievements"`.

**Below** the `h2 element` with the `text content` of `"Achievements"`, I **add** an `h3 element` with the `text content` of `"Presenter 2017"`. The `h3 element` ***more specifically*** describes my **achievements**.

**Below** the `h3 element`, I **add** a `ul element`.

**Inside** the `ul element`, I **add** ***two*** `li elements` with **links** to the `slide decks` I **created** and **used** in the **presentations** I ***made*** in `2017`.  My `ul element` with the ***two*** `li elements` **inside** ***pointing*** to my `slide decks` on `Github`, look like the **following**:

```html5
<ul>
	<li>
		<a href="https://interglobalmedia.github.io/react-workflow-updated-2018/#/"
		   target="_blank"
		   rel="noreferrer noopener">React
			Workflow Presentation React NYC Meetup
			9.28.17</a>
	</li>
	<li>
		<a href="https://interglobalmedia.github.io/evolution-in-design-and-development/#0"
		   target="_blank"
		   rel="noreferrer noopener">Evolution
			in Design & Development React Camp
			11.18.17</a>
	</li>
</ul>
```

**Inside** the `a elements` which **point** to the `URLs` of my `presentation slide decks` on `Github`, I have **added** a `target attribute` with the `value` of `"_blank"`. This `value` **opens** the **targeted** `URL` in a **new tab** or **window**. I have ***also added*** the `rel attribute` with the `value` of `"noreferrer noopener"`. This was **as per** the **suggestion** of `Lighthouse` under `"Best Practices"`, when I **tested** my `resume.html` **page** for `Performance`, `Best Practices`, `Accessibility`, and `SEO`.

The `value` of `"noreferrer noopener"` for the `rel attribute` is **used** to ***prevent*** the **new tab** created by the `value` of `"_blank"` for the `target attribute` from **taking advantage** of the **JavaScript** `window.opener` **feature**. Remember I **discussed** this in the [Sectioning HTML](https://github.com/interglobalmedia/sectioning-html/blob/master/sectioning-html.md) `slide deck` in the `slide` entitled `Commonly used a element attributes`?

To ***recap***, there I **state** that one **should add** the `rel attribute` to the `a element` with the `value` of `"noreferrer noopener"` to `opening a tags` that **point** to `cross-origin URL`s (as **opposed** to **same origin** `URL`s which are ***internal*** to a **site** and ***share*** the **same origin**) to ***avoid exploitation*** of the [window.opener API](https://developer.mozilla.org/en-US/docs/Web/API/Window/opener) (**security move**).

If `rel="noreferrer noopener"` is ***not added*** to the `opening a tag`, the (`browser`) `Window`'s `interface opener property` **returns** a **reference** to the `window` that **opened** the `window` **using** the `target attribute value`. This is ***not*** the **best behavior** as it **poses** a **security issue**. By ***default***, when you **open** a **web page** in a ***new tab*** by `clicking` on a `link` **containing** `target="_blank"`, this page now has **limited access** to the **linking page**. **Nowadays**, with `Firefox 79` and **after**, for example, **giving** the `target attribute` the `value` of `"_blank"` ***implicitly provides*** the **same** `rel` **behavior** as **setting** `rel="noreferrer noopener"`. But it **can never hurt** to **add** `rel="noreferrer noopener"` **just** in **case**, since one **should cover** all **browser bases**, and ***not just*** `Firefox`.

By **adding** `rel="noreferrer noopener"`, I **significantly increased** my `Best Practices` **ranking** in `Lighthouse`.

**This** is what my ***complete*** `"achievements"` **aside widget** looks like:

```html5
<section class="achievements">
	<h2>Achievements</h2>
	<h3>Presenter 2017</h3>
	<ul>
		<li>
			<a href="https://interglobalmedia.github.io/react-workflow-updated-2018/#/"
			   target="_blank"
			   rel="noreferrer noopener">React
				Workflow Presentation React NYC Meetup
				9.28.17</a>
		</li>
		<li>
			<a href="https://interglobalmedia.github.io/evolution-in-design-and-development/#0"
			   target="_blank"
			   rel="noreferrer noopener">Evolution
				in Design & Development React Camp
				11.18.17</a>
		</li>
	</ul>
</section>
```

</section>

---

<section class="section">
	<h2 class="sentence">The "interests" aside widget</h2>

**Next**, **below** the `closing section tag` for the `"achievements"` **aside widget**, I **add** an `opening section tag` with the **class** of `"interests"`. Then I **create** a `closing section tag`. Then, **making sure** that the `cursor` is **placed between** the `opening` and `closing section tags`, I **press** the `return key` and **take** the `closing section tag` to the **next line**.

**Below** the `opening section tag` with the **class** of `"interests"`, I **add** an `h3 element` with the `text content` of `"Interests"`.

**Below** the `h3 element` with the `text content` of `"Interests"`, I **add** a `ul element`. **Inside** the `ul element`, I **add** one `li element` with `text content` **describing** my **interests**.

My ***complete*** `"interests"` **aside widget** looks like the **following**:

```html5
<section class="interests">
	<h3>Interests</h3>
	<ul>
		<li>When I’m not coding, I love to go to the
			countryside
			to recharge, watch Film Noir and mystery movies,
			listen to alternative and soul music, ponder
			over
			surrealist art, and create exotic cuisine.</li>
	</ul>
</section>
```

**Below** this `section element` with the **class** of `"interests"` is the `closing aside tag`, **followed by** the `closing div tag` of the `div element` **containing** the **class** of `"resume_skills"`.

</section>

---

<section class="section">
	<h2 class="sentence">The resume footer and the contact info section</h2>

**Right below** the `closing div tag` of the `div element` with the **class** of `"resume_skills"`, I **add** an `opening footer tag`. Then I **create** the `closing footer tag`. Then, **making sure** that the `cursor` is **placed between** the `opening` and `closing footer tag`, I **press** the `return key` and **take** the `closing footer tag` to the **next line**.

**Below** the `opening footer tag`, I **add** an `h3 element` with the `text content` of `"Contact Maria D. Campbell"`.

**Inside** this `contact info section`, I **add** a `tel: URL scheme` for **making calls** to `mobile devices` from **web pages**, and an `email: URL scheme` for **sending emails** from **web pages**.

**Below** the `h3 element` with the `text content` of `"Contact Maria D. Campbell"`, I **add** an `opening section tag` with the **class** of `"contact-info"`. Then I **create** a `closing section tag`. Then, **making sure** that the `cursor` is **placed between** the `opening` and `closing section tags`, I **press** the `return key` and **take** the `closing section tag` to the **next line**.

</section>

---

<section class="section">
	<h2 class="sentence">The footer contact info section and the tel: URL scheme</h2>

**Below** the `opening section tag` with the **class** of `"contact-info"`, I **add** an `opening p tag` with the **class** of `"tel"`.

**After** the `opening p tag` with the **class** of `"tel"`, I **add** an `opening strong tag` **ollowed by** an `opening span tag` with the **class** of `"type"`. The `opening span tag` with the **class** of `"type"` is **followed by** the `text content` of `"Cell"`. The `text content` of `"Cell"` is **followed by** a `closing span tag`, **followed by** a `:` and ***then*** a `closing span tag`. The `closing span tag` is **followed by** a `closing strong tag`.

**After** the `closing strong tag`, I **add** an `a element`. **Inside** the `opening a tag`, I **add** the `href attribute` with the `value` of `"tel:+xxx-xxx-xxxx"`. This is **called** a [tel: URL scheme](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/a) and is **supported** by `browsers`. This `value` **permits you** to **make** a `phone call` on the `web` via `phone numbers` ***associated with*** `mobile devices`.

My `p element` for the **tel number** to **call** looks like the **following**:

```html5
<p class="tel"><strong><span
			  class="type">Cell</span>:</strong>
	<a href="tel:+1-646-820-7539"
	   target="_blank"
	   rel="
	   noreferrer
	   noopener">1-646-820-7539</a>
</p>
```

</section>

---

<section class="section">
	<h2 class="sentence">The footer contact info section and the email: URL scheme</h2>

**Below** the `closing p tag` of the `p element` with the **class** of `"tel"`, I **add** an `opening p tag` with the **class** of `"email"`. The **structure** of this `p element` is the ***same*** as for the `p element` with the **class** of `"tel"`. The ***difference*** is that this ***regards*** `sending emails` **instead of** `making calls` to **mobile devices**.

My `p element` with the **class** of `"email"` looks like the **following**:

```html5
<p class="email"><strong>Email:</strong> <a
	   href="mailto:interglobalmedia@gmail.com"
	   title="Email Maria D. Campbell"
	   target="_blank"
	   rel="
	   noreferrer
	   noopener">interglobalmedia@gmail.com</a></p>
```

**Below** the `closing p tag` for the `p element` with the **class** of `"email"` is the `closing section tag` for the `section element` with the **class** of `"contact-info"`.

</section>

---

<section class="section">
	<h2 class="sentence">A note about making calls on the web and zoom</h2>

While I was **testing out** the `tel: URL scheme` I **added** as the `value` of the `anchor element`'s `href attribute`, when I **used** my **cell phone number** as the `text content` for the `anchor element` and **clicked** on the `hyperlink`, it **directed me** to **use** `zoom` to **make** the **call**.  But when I ***either*** `changed` the `text content` to `Click to call` or **used** my `Google Voice` **number** and **also used** the `Google Voice number` as the `text content` of the `anchor element`, I was ***no longer directed*** to **use** `zoom`. ***Somehow*** `zoom` has **figured out** my `cell phone number`, because I ***checked***, and I **don't see** having **provided them** with it ***anywhere***. I could be ***wrong***, that but that is what `SEEMS` to **be** the **case**.

So **how** do they ***do that***? Or **how** do they ***hide*** that **info** so that I ***can't*** easily **remove** it? ***Either way***, I ***don't like it***. I **like** my `Face Time` on my `Apple` **devices**. I'll ***save zoom*** for when I absolutely **need it** for **work** `outside` of **teaching**.

If the `person` ***trying*** to **contact** `you` on your `mobile device` **might have** a `zoom account`, and you ***also*** have a `zoom account`, but you **don't want** the `tel: URL scheme` to **redirect** to `zoom`, ***do not use*** your `cell phone number` as the `text content` of the `anchor element`. ***Either*** make it something like `Click to call`, or **use** a `Google Voice number`, if you have one, **instead**. This way you can ***avoid*** `redirecting` your `tel: URL scheme` to `zoom`. I found that you ***don't even*** have to be **logged in** to `zoom` for the `redirect` to ***take place***!

</section>

---

<section class="section">
	<h2 class="sentence">The footer nav</h2>

**Below** the `closing section tag` for the `section element` with the **class** of `"contact-info"`, I **add** an `opening nav tag` with the **class** of `"footer-nav"`. Then I **create** a `closing nav tag`. Then, **making sure** that the `cursor` is **placed between** the `opening` and `closing nav tags`, I **press** the `return key` and **take** the `closing nav tag` to the **next line**.

**Below** the `opening nav tag` with the **class** of `"footer-nav"`, I **add** a `ul element` which **contains** 5 `li elements`. The **content** of the `li elements` **consists of** an `anchor element` **containing** `hyperlinks` to the `URL`s of ***all*** the **pages** of the `portfolio site`. ***Basically***, it's our `site navigation` in the `footer` as opposed to the `header`. This is because ***adding*** a `header` **containing** the `site navigation` **at** the **top** of the `resume page` would **throw off** the `responsive resume`'s **structure**. ***Besides***, it **looks cleaner** and **more presentable** without a `site navigation` **at** the **top** of the **page**. It would have ***visually interfered*** with the `clean page` **look** of the `résumé`.  My `footer navigation` looks like the **following**:

```html5
<nav class="footer-nav">
	<ul>
		<li><a href="index.html">Home</a></li>
		<li><a href="portfolio.html">Portfolio</a></li>
		<li><a href="resume.html">Résumé</a></li>
		<li><a href="about.html">About</a></li>
		<li><a href="index.html">Contact</a></li>
	</ul>
</nav>
```

**Below** the `closing nav tag` is the `closing footer tag`.

**Below** the `closing footer tag` is the `closing div tag` of the `div element` with the `"page"` **class**.

**Below** the `closing div tag` is the `closing main tag`.

And ***that*** is it for the `HTML markup` of the `resume.html`. ***Next comes*** the **associated** `CSS`.

</section>

---

<section class="section">
	<h2 class="sentence">Related Resources</h2>

+ [CSS element+element Selector: w3schools](https://www.w3schools.com/cssref/sel_element_pluss.asp)

+ [RoleAttribute: Wikipedia](https://www.w3.org/WAI/PF/HTML/wiki/RoleAttribute)

+ [What is WAI-ARIA, what does it do for me, and what not?](https://www.marcozehe.de/what-is-wai-aria-what-does-it-do-for-me-and-what-not/)

+ [HTML Symbols: w3schoola](https://www.w3schools.com/html/html_symbols.asp)

+ [`<time>`: MDN](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/time)

+ [CSS Combinators: w3schools](https://www.w3schools.com/css/css_combinators.asp)

+ [`<a>`: The Anchor element](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/a)

</section>

---
