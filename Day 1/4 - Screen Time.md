## Screen Time
### [Luke Wroblewski](https://twitter.com/lukew)

### Introduction
Talks about the creation of Gorilla Glass; didn't have a use case until Steve Jobs realized the usefulness of it. 

> We care about [the display] because that's the window to the software. 
> 
> -- <cite>Tim Cook</cite>

Luke mentions window to the software, [and the web].

### The Screen

Lots of screens, all different dimensions, are being sold. 

* Small (16%)
* Medium (69%)
* Phablets 
* Small (Tablets)
* Full-size (tablets)

#### Activity

Small mobile screens only get used by 7%. 

#### Sessions

Small smartphones - 4%
Medium smatphones - 76%

Not just the quantity of smartphones, but sessions and activity. 

#### 2017 Forecast

> Mobile is the first time the consumer tech industry has  sold to every single person on earth
> 
> -- <cite></cite>

> … not just the size but the resolution, the clarity, […] we care about all those
> 
> -- <cite>Tim Cook</cite>

### Higher Resolution Displays

* SD (4:3)
* HD (16:9)
* Full HD (720p)
* Ultra HD
* 4K (19:10)

As resolutions continue to grow, our designs actually are/should be impacted. 

#### "Solutions"

* Use CSS & Web type whenever possible
* SVG & Icon fonts whenever applicable
* Picturefill raster graphics
	* `<picture>`
* Media queries
	```css
	@media only screen and (min-device-pixel-ratio: 1.5) { … }
	```
	
Netflix and Youtube are 50% of downstream bandwidth (e.g. 50% of data).

### Orientation

65% landscape | 35% portrait (tablets)

#### Vertical Media Queries

> [increase font size] on screens that are wide enough but not tall enough for it to make sense.

* Tighten up the padding/margins
* Move up the call to action(s)
* Make sure image/content is still visible as height decreases

#### Portrait "App"

Uses off canvas menu navigation, and a bottom menu instead of a side menu

* Trend towards high resolution
* Trend towards widescreen aspect ratios
* Media queries are more powerful than just width

### Input

> Any piece of glass you can't touch and interact with will feel broken.
>
> -- <cite>Microsoft guy</cite>

Illustrates various capabilities of mobile/tablet devices, e.g.

* Multi-touch
* Pen
* Keyboard
* Cursor
* etc.

> Can't we just detect input type & change the interface?

> Don't attempt to switch between keyboard and touch.

Solution he went with was just to detect screen size, no good solution to detect touch. Use tips (for keyboard) when resolution gets large enough.

#### Media Queries (Level 4)

* pointer: input being used; `cursor`, `finger`, `stylus`
	```css
	@media (pointer:coarse) { … }
	```
* hover: will hover pseudo-class work on the current device?

#### Input

* Support **all** the inputs
* Communicate what's possible
* Screen size is a poor proxy, but it's all we have *(for now)*

### Posture

(How people interact with output & input)

Netflix is concerned with viewing distance; "10-foot guy", "2 foot guy", "18 inch guy"
- 18 inch guy is tablet/mobile viewing distance
- 10 foot is regular viewing distance for television

If they tried to turn to targeting device they would have a rough time; instead turned to human factors.

- 10 ft
- 2 ft
- 1 ft
- 1.5 ft

Mobile: Box art is sized 1"
Tablet: Box art is sized 1.75"
Laptop: Box art is sized 2.25"
Television: Box art is sized 5.25"

(Roughly .5" / ft.)

#### Google Glass

Webpages are designed more like they would be for a television screen.

Screen size is a poor proxy for detecting posture.

(Media Queries level 4)

* light-level: the ambient light-level in which the device is used
 ```css
 @media (light-level: washed) { … }
 ```
 
 * Design to human scale
 * And environments
 * Not just screen width
 
 ### Wrap-Up
 
 Web is better suited for these adaptive techniques, via media queries.
 
 1. Know your screen
		* Online time is screen time and increasingly mobile
	2. Output
		* high resolution & widescreen
		* Vertical Media queries
	3. Input
		* Support all inputs
		* Communicate what's possible
	4. Posture
		* Viewing distance
		* Environment & more
		* Media queries don't help much here… yet

> What material comes after glass? What's the disruption?

* Sapphire (glass)
* Voice interface
	* Has a hard time imagining this is the "future"
	* Opportunities are not nearly as broad as with other input technologies
* Wearables
	* Going to complement smartphone & tablet growth? Or supplant it?

#### Corning
> Flexible glass that is thinner than a dollar bill.


 
 








