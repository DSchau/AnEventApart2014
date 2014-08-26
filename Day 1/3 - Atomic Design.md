## Atomic Design
### Brad Frost

### What is an interface made of?

> Design systems, not pages. - Andy Clarke

Frameworks (like ZURB's foundation) is a system. 

### Issues with Frameworks (Bootstrap, Foundation, etc.)

We have different tastes, experiences, etc. 

* One size fits all
	* Lookalike issues
		* if Nike, Reebok, Puma, and Addidas all used Bootstrap they would look substantially similar
			* If they do look different, they "fought against" the framework
* Potential for bloat/unneeded stuff
* Might not do everything you need
	* End up having to write a bunch of custom code anyways
* Subscribe to someone else's structure, naming, style, etc.

> Tiny Bootstraps, for every client.

> Responsive deliverables should look a lot like fully-functioning Twitter Bootstrap-style  custom tailered for your clients' needs.

### Benefits of Front-end Style Guides

* Promote consistency and cohesion
* Easier to test
* Better workflow
* Shared vocab
* Useful referene

[Code for America](COA)

#### Problems

* Time consuming to create
* Often too abstract
* Seen only as a designer/developer tool
* Created *after* a project launches

### Atomic Design

In natural world, we have atomic elements; each have their own properties. We can take those "atoms" and combine to form molecules. 

Those molecules take on new properties, start becoming more useful. Keep combining to form simple organisms. Combine to form complex organisms. 

All matter in the universe is composed of this finite set. 

[Periodic Table of HTML Elements](PERIOD_HTML)

#### Atoms

e.g. labels, input, button, etc. 

#### Molecules

Take atoms, combine to form a molecule

e.g. search input combined with search button

#### Organisms

Put molecules in context of a larger module, organism; relatively complex thing.

e.g. Navbar

#### Templates

Standalone chunks of "organisms" can be put together in context of page-level element.

e.g. underlying content structure, rather than focusing on final page

> What your content is made from, not what your content is. - Mark Boulton

#### Pages

Take those templates and "pour in" real, representative content. 

Need to be able to solve for dynamic data. 

#### Wrap up

Work from most granular to most complete. 

Abstract -> Concrete

Creators care about the abstract, the clients care about the concrete.

### Pattern Lab

Static site generator that takes components and puts them into a front-end interface. 

#### What it's not

* UI Framework
* Language, library, style, workflow dependent
* Incredibly rigid
* *Just* a pattern ilbrary, but also not a production-ready static site generator













[COA]: http://style.codeforamerica.org "Code for America Style Guide"
[PERIOD_HTML]: 