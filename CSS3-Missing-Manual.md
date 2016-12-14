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

##Chapter 5

##Chapter 6

##Chapter 7

##Chapter 8

##Chapter 9

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

##Chapter 12

##Chapter 13
