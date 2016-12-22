#CSS3: The Missing Manual Notes

##Chapter 1

Use HTML primarily for structure in a page (a.k.a. markup) rather than for formatting content since CSS is more efficient for that purpose. Use the &lt;div&gt; (block) &amp; &lt;span&gt; (in-line) elements, along with the class attribute, to be the primary means for marking content for formatting in CSS. There are also the section, aside, footer, nav, figure, and article tags which act as div tags but have specific purposes.

##Chapter 2

CSS consists of 5 main parts: Selector, Declaration Block, Declaration, Property, and Value.

Selectors are used to identify which part of the html you are formatting. Declaration Block if a section bracketed by {} that contains the Declatations. Declarations are the instructions for how to format the content and consist of properties and values. A property is the formatting option that you are targetting, while a value indicates how the property should display.

Style sheets can be internal or external. If the formatting you are using will NEVER be used on another page, then use the internal CSS. Otherwise, use external. To use internal CSS, just place the CSS code in a &lt;style&gt; element in the head.

##Chapter 3

ID selectors should be used rarely, with class selectors usually being preferred. In general you should try to use the selector that best fits the situation.

Psuedo-Selectors include :hover, :visited, :link, :active, :first-letter, :first-line, :focus, :before, :after, and ::selection.

Attribute selectors are contained in [], such as tag[attr], and target only elements with the tag AND the attribute indicated. When combined with a value, you can get even more specific.

|Conditional|Effect|
|:-:|---|
|=|Must have the exact value|
|^=|Value must start with entry|
|$=|Value must end with entry|
|*=|Value must contain entry|

Child selectors include :first-child, :last-child, and :nth-child(). The () should contain odd, even, or a math expression using "n". Others include :first-of-type, :last-of-type, and :nth-of-type().

Sibling selectors allow you to select elements that are children of the same parent element.

##Chapter 4

Inheritance allows many properties of an element to be passed down to all of its descendants, but generally not those that affect layout and positioning.

##Chapter 5

When inheritance conflicts, the closest ancestor wins. A directly applied style always beats inheritance. For directly applied styles, order of precedence is: Inline > ID > Class > tag, i.e. a class selector supersedes a tag selector. In a tie the last applied style wins. You can add !important to the end of a declaration to give it the highest priority.

In general try to keep selectors short and avoid having all of your selectors compete.

##Chapter 6

If you choose to use a non-standard font, be sure that you have legal permission to use it on your website first. Also use the @font-face 4 times to set up the regular, italic, bold, and bold italic versions of the font.

Colors can be specified in hexadecimal, RGB, RGBA, HSL, HSLA, and named formats.

Capitalization can be controlled with the text-transform: property, while font-variant: can be used for special effects and text-decoration can be used to add lines above, below, or through text. letter-spacing: and word-spacing: control the spaces in text. text-shadow: RIGHT DOWN BLUR COLOR can be used to add text shadows. line-height: can be used to control spacing between lines of text, and text-align: controls the left, right, center, and justified positions. text-indent: will indent lines of text.

##Chapter 7

Margin is the space between elements, and will always default to ONLY the highest margin. Padding is the space between content and border.

border-radius: is used to round the corners on borders. box-shadow: is used to add a shadow to a box, with inset being added as a value to have the shadow appear inside the box. Also, box-sizing: border-box allows you to define the width while including the padding and border, but not the margin. overflow: can be used with the visible, scroll, auto, or hidden values to tell a browser what to do with content that is too large to fit inside of a box.

##Chapter 8

In general it is preferable to use a background image rather than the img tag in html to add an image when possible. Tiling of background images can be used to control appearance, and multiple background images can be used at the same time, such as using 3 images with 1 tiling vertically to create a "scroll" that resizes to fit content. background-attachment: fixed can be used to ensure a background image does not move when the user scrolls down the page.

The linear-gradient(START, COLOR1, COLOR2, etc.) value can be used to create gradients as a background when combined with the background-image: property. Lengths can be added to the colors to denote how far along the image the color should change. repeating-linear-gradient() can be use to create a repeating gradient. Radial gradients can also be created by replacing the "linear."

##Chapter 9

Always place :link, :visited, :hover, and :active in that order for a particular link. Use unordered lists for a navigation bar and then simply remove the bullets and padding/margin.

##Chapter 10

###Transform

The "transform:" property can be used to perform geometric transformations on elements. Needs vendor prefixes (-webkit, -moz, -o, & -ms). It will accept the following values:

|Value|Effect|
|---|---|
|rotate(Xdeg)|Rotates the element X degrees|
|scale(S)|Applies a scaling factor of S|
|scale(X,Y)|Applies scale factors to X and Y axes|
|scaleX(S)|Scales on X axis|
|scaleY(S)|Scales on Y axis|
|translate(Xunit,Yunit)|Translates the elements along the X and Y axis away from the top left by the indicated units|
|skew(Xdeg,Ydeg)|Slants the element the indicated number of degrees along the X or Y axes|

Multiple transformations can be applied, for example: "transform: skew(45deg,0deg) scale(.5) translate(400px,500px) rotate(90deg)".

Center of element is default origin. "transform-origin: Xunit Yunit" can be used to define a different origin for transformations.

Requires vendor tags.

###Transitions

"transition-property:" identifies which property to alter, while "transition-duration:" defines the length of time for the transition to occur in seconds (s) or milliseconds (ms). "transition-timing-function:" can be used to control the speed of the transition, accepting linear, ease, ease-in, ease-out, and ease-in-out. "transition-delay:" can define a waiting period before the transition begins.

Requires vendor tags.

###Animations

Use "@keyframes animationName {}" to begin defining an animation. Requires a "from {}" and "to{}". The from will indicate the initial state while to indicates the final state of the animation. you can use "X% {}" to define where during an animation that a certain state should occur.

To apply an animation, use the "animation-name: animationName" and "animation-duration:" properties. Can also use "animation-timing-function" like transitions. "animation-iteration-count:" can define how many times to run an animation, with infinite making it run on loop. "animation-direction: alternate" can cause an animation to reverse direction each time it plays. "animation-fill-mode: forwards" will cause the browser to keep the end state of the animation instead of reverting to its initial state.

Requires vendor tags.

##Chapter 11

Use tables for actual tables of data, not to arrange content in HTML. Use the &lt;colgroup&gt; and &lt;col&gt; tags at the beginning of a table so you can markup the columns as well as the rows of a table. Each cell in a table will have its own margin, padding, and border. Use border-collapse: collapse to eliminate margins and double borders from cells, but this will disable empty-cells and border-radius properties.

Use a label CLASS (not the tag) to denote the questions for each form area so that you can more easily organize the layout of the form. This is especially true for radio and checkbox, since the label will actually the text associated with each individual response. Then apply the display: inline-block and width: properties to align the form in a way that is pleasing to the eye.

##Chapter 12

The 3 main types of layouts are Fixed, Liquid, and Responsive. Fixed uses pixel lengths for elements so that a web page always displays the same way no matter how big or small a screen is. Liquid uses percentages so that content is resized to fit the size of the screen. Responsive is designed to detect the browser settings and automatically adjust the layout to a preset tailored for the screen size.

The major key is to use the HTML to organize content with semantic tags, then use CSS to arrange it using such properties as float. Sketch the layout of your page on paper first then see about how to realize that layout using boxes. After you have everything positioned the way you want, then start adding borders, images, and colors.

##Chapter 13

Float is very useful for positioning a box to the left or right edge of its parent box, but always be sure to specify a width for floated boxes. By using multiple levels of floated boxes you can create more complex multi-column layouts. Use the clear property to ensure that no other siblings are on the corresponding side of the box.

Background images can be used in a wrapper box to "fake" column backgrounds that extend below the content of the column; just use gradients.

Be careful about box sizing to prevent float drop, which is when a float seems to inexplicably drop below content that it should be next to.

##Chapter 14

Responsive Web Design (RWD) is a series of html and css techniques that allow a site to automatically adjust its layout depending on the device being used to access it. To prevent phone zooming with RWD use &lt;meta name="viewport" content="width=device-width"&gt; in html OR @viewport {width=device-width;} in css.

Good changes to make based on device are: # of columns, flexible widths, white space, font sizes, navigation menus, and background images. It can also help to cut some content from a page when being viewed on a small device.

To make a media query in html, you use the media attribute inside a link element. The format is: media="(dimension:Xpx)" where X is a number and dimension can be min-width, width, or max-width. Use "and" to connect multiple media queries to create a width range. You can import an external CSS file using @import url(URL) (dimension:Xpx); or by using @media (dimension:Xpx) {} with all of the styling done in the declaration block.

The width: and max-width: properties can be used to easily create automatically sizing boxes, but be sure to set box-sizing to border-box first.

##Chapter 15

Four positioning values: Absolute (removes from flow, position from top, left, bottom, and/or right), Relative (same as absolute except not removed from flow), Fixed (locks position on screen regardless of scrolling), and Static (default). When using anything other than static, it will default to the top-left corner unless you specify its position.

Both absolute and relative position are always relative to the parent box. Use relative divs inside of absolute divs to aid in layout.

To hide an element, use "display: none" or "visibility: hidden" or "opacity: 0". Combined with :hover you can use this to display captions when a user mouses over an image.

Fixed positioning is useful if you want to keep certain elements always on the screen in the same place, such a a company logo or navigation bar, but be sure to position other elements with margins to prevent overlap.

##Chapter 16

Use comments to denote the purpose of declarations so that you can easily identify what you were doing at a later point. Name your classes and IDs clearly so it is obvious what they are, focusing on purpose rather than appearance or position as those may change later. Use multiple classes for to be able to apply styling selectively and avoid re-typing css code that appears already in your code.

In the CSS file determine a standard way to organize your styles, either by related content or by purpose, and use comments to separate and name them. You can also create multiple CSS files each with a specific purpose to prevent a single CSS file from becoming huge and unwieldly. Then simply use a singe CSS file that imports each of the other CSS files.

To help your site look the same in all browsers, it can be helpful to "zero-out" the default formatting. This can include removing padding and margins, applying consistent font styles, making everything display as a block by default, setting a consistent line height, customizing tables, removing borders from linked images, setting consistent list formatting, and removing quote marks from around quoted material.

Use descendent selectors when appropriate instead of creating a class for every element. Use a div wrapper for major content areas with a class applied, then use descendent selectors to find elements within that div. Applying a class to the body tag can allow you to customize content by page easily using descendent selectors.

You may also need to create specific css styles for Internet Explorer versions using: &lt;!--[if IE X]&gt; html code &lt;![endif]&gt; where X is the IE version, and removed if applying to all versions of IE.

##Flex

display: flex; - creates a flex container.

flex-direction: column/row; - column for horizontal division, row for vertical division.

flex-grow: # - defines a flex item and what ratio of unused space it should use.

flex-shrink: # - defines a flex item and what ratio of excess space it should lose.

flex-basis: 

flex-order:
