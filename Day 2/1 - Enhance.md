## Enhance
### [Jeremy Keith]()

### Introduction

Begins with visual examples to "re-wire your brain," e.g. a picture of a duck and then he points out "all ducks are wearing dog masks," Fedex & Toblerone logos, etc.

We had to learn to use the web, it wasn't necessarily an easy concept to wrap your head around.

> Killer Web Sites' are usually those which tame the wildness of the web, constraining were made of paper--Desktop Publishing for the Web
>
> -- <cite>John Allsopp</cite>

New medium tends to take on the tropes of existing medium (e.g. internet often inspired by print).

### HTML

Progressive enhancement: Layers of structure (HTML), presentation (CSS), and functionality (JS)
 - more relavant today than it ever has been

#### Shearing Layers

You can move furniture around, but it's much more difficult/time-consuming to change the walls. 

Instead of thinking of technology as a bundle, think of it as layers that depend on other layers. 

#### HTML

Fault tolerant structure, e.g. `<blorp></blorp>` will still render

Structural honesty: e.g. Use a `<button></button>` element instead of `<span></span>`

#### CSS

```css
selector {
	property: value;
}
```

Does not stop parsing the CSS if there's an error (fault tolerance)

Material honesty: use border-radius on an element, not a hacky 4 span structure

#### Javascript

Not fault-tolerant. 

> When an elevator fails, it's useless. When an escalator fails, it becomes stairs. We should be building escalators, not elevators.
>
> -- <cite>Jake Archibald</cite>

With Javascript, it's very easy to create a single point of failure. 

> Progressive enhancement is more about dealing with technology failing than technology not being supported.
>
> -- <cite>Andy Hume</cite>

#### gov.uk

Found that 0.9% of their users didn't have Javascript enabled/active (for some reason). In a year, that means that 3,391,200 people aren't able to access the site. 

> If you build pages with the idea that parts other than HTML are optional, you will create a better and stronger web page.

Robustness principle:

> Be conservative in what you send; be liberal in what you accept.
>
> -- <cite>Jon Postel</cite>

### Design Principles

Design patterns can be seen in the Declaration of Independnce, Asimov's robotic principles, etc. 

> Software, like all technology, is inherently political. Code inevitably reflects the choices, biases, and desires of its creators.
>
> -- <cite>Jamais Cascio</cite>

All software is opinionated; have to figure out if tool's philosophy matches your own. 

### JS Frameworks

Order of opinonated-ness, ability to use along with progressive enhancement.

1. Backbone
2. AngularJS
3. Ember

They rely on Javascript, the one point of failure for most applications, not fault-tolerant portion.

> No one wants to think that what they're doing is trivial.
>
> -- <cite>John Resig</cite>

Building elevators, not escalators. 

### The Web Platform

e.g. other platforms are flash and native

However, he doesn't like the term, compares it to similar terms like "friendly fire," "mobile web," "tax relief," etc.

Thanks to progressive enhancement (layered structure), pretty rare that someone will get 0% of your content if building site correctly. The web is not a platform, it's cross platform. 

Framing of the web as a platform is a category error. 

> It's hard not to be disappointed by HTML if you've developed for iOS, Windows, or other mature platforms as I have.
>
> -- <cite>Joe Hewitt</cite>

Don't think of the verbs that don't matter (swipe, tap, drag, etc.) but think of the action verbs associated (e.g. publish, find, buy, share)

### Website vs. Web Apps

Just doesn't understand purpose of delineation into two buckets. 

Gives that assocation that a "web app" is something more powerful than a website (e.g. what you're doing is "more complex").

Used as a "get out of jail free" card so that you can not worry about accessibility and those kind of things

### Passive vs. Interactive

If you're designing something passive, need to especially focus on contrast, white-space, type, etc.

Difficult to really find where your website really is

### Responsive Enhancement

Treating layout as an enhancement

Fluidity is inherent to the web

Stop thinking about "how do I make my website responsive," but instead frame it as "How do I keep my website responsive?"

> The web is responsive on its own--by default. It's us that's been breaking it all these years by placing content in fixed-width containers.
>
> -- <cite>Andy Hume</cite>

#### Do websites need to look exactly the same in every browser?

(NO)

### Cutting the Mustard

```js
if ( document.querySelector && window.addEventListener ) { … }
```

Feature detection, not browser detection. 

### Aggressive Enhancement

Should support *every* browser, but don't need to optimize for every (or any) browser. 

> There is a difference between support and optimization.
>
> -- <cite>Brad Frost</cite>

#### Don't waste your time making websites look the same in every browser

Best way to be future-friendly is to be backwards compatible. 



