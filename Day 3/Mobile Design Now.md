## Mobile Design Now
### Luke Wroblewski

### Introduction

#### Chart of Luke's Mobile Path

- Mosaic web browser (1995 NCSA)
	- 50 million -> 150 million PCs in 3 years
- The bubble popping (2000 - 2001)
	- Global sales didn't necessarily collapse, just leveled off
- Took a job at eBay, then yahoo in early 2000s
	- Designed yahoo's home page
- End of 2009 resulted in biggest drop ever in history of PC sales
	- Significantly larger drop than in early 2000s
	- Smartphones and tablets seem to explain this drop
	- This is the "Mobile Moment"

### The Mobile Opportunity
#### Mobile Moment
Many companies had their "mobile moment" (when traffic/revenue/etc. shifts to mobile) in the last couple of years; Amazon, ESPN, YouTube, etc.

#### Desktop Navigation
**W**indows
**I**cons
**M**enus
**P**ointers

PC lifespan (continuing) - 29 years
Mobile - 6-7 years

#### Issues with Desktop -> Mobile

##### Amazon
Moved to a native iOS application

- Same experience "shrunk down"
	- Same data, just with slight mobile enhancements
	- This approach is what stems from 30 years of designing desktop products

Amazon Flow: "A magical shopping wand for the world"

A *much* different experience compared to Amazon's earlier efforts with mobile shopping.

Amazon's technique tends to be to use mobile "test" applications, improve the functionality, and then fold it into the application.

#### Desktop -> Mobile

There is much to learn (w/ mobile) but also much to unlearn w/ desktop

### Design Considerations
Number of different ways to make design decisions:

- Product vision
	- Central idea or concept
		- e.g. the product vision of Yahoo was a dashboard
- Design principles
	- Characteristics used to evaluate decisions
		- e.g. Facebook's "universal, human, clean, consistent, useful, fast, transparent"
		- e.g. Google's "design for the world, add a human touch, delight the eye without distracting the mind, every ms counts, be worthy of people's trust"
		- e.g. Microsoft's "focus should be on content; not ui, reduce number of choices presented at any given time, increase efficiency, embrace consistency, give features a permanant home, etc."
	- Can be useful if they're specific to what you're trying to achieve
	- High level "nebulous" characteristics aren't particularly helpful
- Design patterns
	- Repeatable solutions in context
		- *Needs* to address context, otherwise it's not particularly useful
	- Component library doesn't necessarily tell you how to solve a problem
- Design considerations
	- How/what to think about while designing

### (Mobile) Design Considerations

- Help shake off PC tendencies
- Create in a mobile "native" way
- Make informed decisions

### Layout & Navigation
How do we organize and present information on mobile?

#### Think outside the display box
Just doing a one-column display does not suffice

It's not that scrolling is bad, necessarily.

- People will scroll through primary content
- Secondary content can be off-canvas
	- But available when you need it

##### Off-canvas design patterns

Has been re-appropriated oftentimes with navigation

There's also an above menu pattern

> Off canvas navigation is especially effective for complex/deep structures.



#####  The Fold
"We need the call to action above the fold so it's obvious and clickable"; 30% higher conversion with a longer page

> The issue isn't whether the cal to action is visible. The issue is whether your call to action is visible at the point where someone has become convinced to take action.

> Scrolling is a continuation; clicking is a decision.
>
> -- <cite>Josh Porter</cite>

#### Obvious Always Wins

##### Hamburger Icon
- [Mr. Liney](https://twitter.com/MrLiney)

Rationale:

- Everybody is doing it now, so people get it
- Facebook trained a billion people on how to use it

> compared on: engagement, satisfaction, revenue, speed & perception of speed metrics; hamburger icon was outperformed by tab bar

Most people don't know what it is/does, thought it might be an "Apple thing."

###### James Porter's Results
> MENU was selected by 20% more unique visitors than the icon

###### Navigation Drawer
Engagement dropped by half compared to tabs

###### Time.com redesign
Started with a hamburger icon, added MENU text, added a callout, etc.

Seems obvious that traffic was down with the change, so attempt to draw attention.

___

Don't just copy "patterns"

Don't assume that other, larger companies know what they are doing

##### Segmented Controller

Switched to a toggle menu; engagement went way down

##### Carousel
Less than 1% of visitors to ND would click the carousel

Amazon has a cool solution

### Input & Actions

- How do we allow people to get things done?

#### Minimize typing mistakes
> In general, using input elements is dificult for users. Avoid text input where possible.

> The rule of thumb is to limit the use of forms in the mobile context.

> Filling out forms for web based services on mobile devices is a very time consuming and frustrating task for users.

##### Input formatting / validation
- Removes placeholder
	- 99% of job postings (at a certain site) just submitted the placeholder as value
- Inline validation
	- > Did you mean luke@gmail.com?
	- Real time feedback; visual symbols
- Alert on form submission
	- > Does your e-mail address look right? 
- `<input type="email">`
	- `autocapitalize="off"`
		- Words
		- Characters
		- Sentences
	- `autocorrect="off"`
- Input masking
	- Avoid the gradual reveal
	- Password masking
		- > Masking passwords doesn't even increase security, but it does cost you business due to login failures
		- Tap a button to show password; or swap behavior and "hide password"
- Allow people to verify sensitive information
- Input prompts
	- Focus on first input
	- Focus on first action (e.g. camera view)
		- Twitter focuses on image on new tweet display
- Input actions
	- comment form above keyboard
	- iOS form actions
- Button inputs
	- Series of inputs that can be clicked to autofill a certain category

###### Condense Input Controls
1. Smart defaults
	* Open table picker menu
	* Table for 2; current date; current time
2. Keep people in input mode
	* One place to provide a set of information (e.g. multi selector)
	* Full name instead of first/mi/last
3. Hide irrelevant controlers until/if they need them
4. Avoid splitting single input entities
	1. Have hard time navigating between fields
	2. `<input type="text" pattern="[0-9]*">`
5. Be mindful of existing conventions

###### Make Primary actions obvious
- When an action is important, it should look that way

##### Dropdowns are the UI of last resort
- Could use a stepper instead
- Could use an action sheet (dialog or popup)

### Feedback & Communication
How do we let people know what is happening?

####  Focus on progress, not indicators
- Default spinner is akin to waiting in a doctor's office and having a phone shoved in your face

##### Ways to prevent
- Skeleton pages
	- Load data into a "wireframe"
	- More applicable when there's a longer wait
-  Interface transitions
	- Use animations/other tricks to make user think it's faster than it actually is; something happens

#### Make apps feel faster
- Amazon
	- 100ms delay results in 1% sales loss
- Yahoo
	- 400ms delay results in 5-9% drop in full page traffic
- Google
	- 500ms delay drops search traffic by 20%
- bing
	- 1s delay results 4% drop in revenue

- Provide instant feedback
- Perform actions optimistically
	- e.g. Instagram assumes a "like" will be successful prior to getting server callback
- Move bits while no one is watching

#### Teach in the moment
- Introduction "tests" (tours) are bad
	- Up-front owner's manual shoved in your face
	- > Help & tips are not bad UI but how they are implemented usually is

Prefer just-in time tips

