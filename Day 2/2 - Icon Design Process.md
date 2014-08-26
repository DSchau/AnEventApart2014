## Icon Design Process
### [Jon Hicks]()

### Introduction

Bringing "The Icon Handbook" up to date, as it was written two years ago

### How do we use icons?

* Gives the eye something very easy to scan, read, etc. 
* functions, e.g. closing a window, play, etc.
* Overcoming language barriers
	* e.g. "hamburger" icon for menu (club sandwich)
* Feedback
	* Also important to use icon and color
* Express emotion/mood

### Where do icons come from?

* Form of visual language before written language
	* e.g. a cave pictograph of the sun
* 1880s - Hobo network
	* Developed series of icons for things like "dangerous neighborhood," "kind lady lives here"
* Xerox Star (1974)
	* First GUI, icons, etc.
	* David Canfield-Smith
	* Icon is more than image; embodies properties that it represents
		* "Likeness or image" (Greek)
		* Pictogram
* Apple (1984)
	* Susan Kare's icons

[Iconic](useiconic.com)

### Why make your own?

* May not be the right size
* May not be the right style
* Too many "spare" icons
	* e.g. only need 6 "specialist" icons
* May not have the right icons

### Icon Creation Process

* Research
* Drawing
* Deployment

### Research

Usually starts with an icon audit; Can sometimes reveal areas of inconsistency

#### Discovery Phase

* Pick 6 icons from the icon audit list; concentrate on those
	* For each of those, decide what the metaphor will be

Iconic: represents the object (e.g. phone)
Symbolic: Meaning has to be learned (e.g. refresh)

Conventions make it much easier (e.g. RSS is now a convention, Home icon is generally a convention, etc.)

### Style

As simple as possible, but no simpler. 

### Tools

He prefers Illustrator; mentioned Photoshop, Inkscape. 

### Grid

#### Balance
Don't have to fill up the entire bounding box.

Can create a "safe area" that you should stay within

#### Space
Can effectively use negative space.

Can suggest a shadow with negative space

### Deployment

#### Easy, with fallback

```html
<img src="twitter.svg" onerror="this.src=twitter.png">
```

Negative is that the .png should be the default (progressive enhancement).

#### Better

```html
<a href="https://twitter.com/foo">
	<i class="icon icon-twitter"></i>
	Follow us on Twitter
</a>
```

#### Why use iconfonts?

1. One small file
	* Different font files for different browser
2. Accessible & scalable
3. Easily styled with CSS
4. No sprites
5. Supported in every browser (IE4+)

#### Why not iconfonts?

1. Bad process (to deploy/make/etc)
2. No meaning
3. Only monochrome
4. No font = no joy
5. Rendering inconsitencies
6. No meaning

Browsers without @font-face;

1. Opera Mini
2. Nokia XPress
3. Blackberry 4 & 5
4. Android 2.1
5. Windows Phone 7 - 7.8

Total estimate: 370 million

#### Tools for iconfonts

Glyphs app

#### Why use SVG?

1. Less hassle
2. Fairly good support (3 versions back of all browsers)
3. Avoids sprites
4. Multiple colors
5. Still style-able with CSS
6. Animations

#### "Future" of SVG techniques

Off canvas SVG, with inner reference to existing SVG

#### Best solution

Grunticon

