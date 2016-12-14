#HTML & CSS Notes

## HTML

###Chapter 1

1) Structure is important to aid in the flow of information for a reader.

2) Elements are designated by "&lt;" and "&gt;" brackets and will have an opening and closing tag.

3) A "/" in a tag designates the closing tag.

4) Information between opening and closing tags have rules applied to them as indicated in the "Tags" section.

5) Templates can be used to simplify and streamline website editing.

6) View Source can be used on a website to view the html code of the web page.

7) Code management systems allow html code to be more easily managed and edited.

###Chapter 2

1) Structural markups manage the structure and appearance of text.

2) Semantic markups provide extra information about content.

3) Maintain awareness of white space collapsing: multiple spaces and/or a single line break collapse to 1 space.

4) Visual editors can provide shortcuts for html coding.

5) Empty elements close themselves and always include a / at the end.

###Chapter 3

1) Lists can be created within lists to create sub-lists.

2) List format:

&lt;ol&gt;
  &lt;li&gt;Item 1&lt;/li&gt;
  &lt;li&gt;Item 2&lt;/li&gt;
&lt;/ol&gt;

###Chapter 4

1) Index.html is the default site in a directory if unspecified.

####Href uses

  A) If linking to another website, use the full url.

  B) If linking within a website to another page, domain name is not necessary. Relative URLs can be used as shortcuts if predefined.

####Relative URLs:

  A) Same Folder: Use file name.

  B) Child Folder: Use file path and name.

  C) Parent Folder: Use "../" to indicate going up a file level.

  D) Root Folder: Use "/" to return to root folder.

###Chapter 5

1) Use separate folders to store images for organizational purposes, especially if the images may be used on multiple pages.

2) Where you place the code for an image will determine where it displays on the web page.

3) Save images at the same height/width that you plan to display.

4) Most computer screens have 72 pixels per inch; keep in mind when deciding what resolution to save with.

5) Use jpeg when saving an image with many different colors, even if only subtly different.

6) Use gif or png for images with few colors and/or large areas of the same color.

7) Bitmap images (jpeg, png, gif) store images as pixels.

8) Vector images (SVG) are pixel independent and can be easily scaled w/o loss of resolution.

9) Animated gifs display several gif frames in sequence, best used for simple illustrations.

10)Gif and png files can be transparent within certain restrictions.

###Chapter 6

1) The elements thead, tbody, and tfoot are typically used only for long tables.

2) Format of a table:

&lt;table&gt;

  &lt;tr&gt;

  &lt;td&gt;Cell 1A&lt;/td&gt;

  &lt;td&gt;Cell 1B&lt;/td&gt;

  &lt;/tr&gt;

  &lt;tr&gt;

  &lt;td&gt;Cell 2A&lt;/td&gt;

  &lt;td&gt;Cell 2B&lt;/td&gt;

  &lt;/tr&gt;

&lt;/table&gt;

###Chapter 7

1) Forms allow users to input data into a website.

2) Various types of forms: Text input (single line of text), Password input (text input with hidden characters), Text area (allows multiple lines of text), Radio buttons (select exactly one choice), Checkboxes (select any number of options), Drop-down boxes (pick one option from a list), Submit button (used to submit data), and File upload (used to upload files).

3) Once a radio option has been selected, the user cannot unselect it. They can only select another option.

4) Labels are best placed above or to the left for text, textareas, select, and file; best placed to the right for checkboxes and radio.

5) Get will attach form values to the end of the url in the action, best used for small amounts of information that will not be added/deleted from a database.

6) Post will send form values as HTTP headers, best used for larger amounts of information or when it will be added/deleted from a database.

###Chapter 8

1) Comments are written in HTML in the format: &lt;!-- write comment here --&gt;.

###Chapter 9

1) Javascript is the most popular way to add Flash to a webpage.

2) Div can be used to create a space for a Flash movie and provide alternative content for those that cannot play Flash.

3) External hosting, like Vimeo and Youtube, may be used but come with potential issues such as advertising and privacy.

4) To host a flash video, first convert to FLV format, then install a FLV player, and finally include the player and the video in your page using JavaScript.

5) To use HTML5 video, you first need to convert to H264 and WebM formats.

6) To play audio, you can use a hosted service (soundcloud.com), use flash, or the HTML audio element.

|Tag/Attribute|Purpose/Effect|
|---|---|
|&lt;video&gt;|Used to encode a video|
|&lt;audio&gt;|Used to embed audio into a webpage|
|preload="none/auto/metadata"|Tell browser whether to load the video/audio while the page loads|
|src="URL"|Tells browser where to find the video file|
|poster="URL"|Displays a default image until video starts playing|
|width/height="number"|Specify width/height of video|
|controls|Tells browser to use its own controls for playback|
|autoplay|Tells browser to automatically play the video/audio|
|loop|Tell browser to loop the video/audio|
|&lt;source&gt;|Used with src attribute to specify location of video/audio file, do not use src with both the video/audio and source elements, can be used to indicate multiple video/audio formats|
|type='format'|Used with &lt;source&gt; to indicate the video format|
|codecs="codec"|Used within the type attribute to denote the codecs used|

### Chapter 10

1) To use a CSS file, the following must be contained in the &lt;head&gt; element:

&lt;link href="(css file)" type="text/css" rel="stylesheet" /&gt;

2) Comments are written thusly: /* comment */

3) CSS allows you to define how certain elements in html should be displayed.

4) Last Rule: If selectors are repeated, the last one takes precedence.

5) Specificity: The most specific rule takes precedence.

6) Importance: !important after a property value gives it max precedence.

|Selector|Meaning|Example|Function|
|---|---|---|---|
|Universal Selector|Applies to all elements|* {}|All elements on page|
|Type Selector|Applies to matched elements|h1, h2, h3 {}|Only h1, h2, &amp; h3 elements|
|Class Selector|Matches only elements with the class after the period, can be set to only one type of element|.note {} or p.note {}|Note class elements or p elements with the note class|
|ID Selector|Applies only tot he element with the matching ID|#introduction {}|Element with the introduction ID|
|Child Selector|Applies only to elements directly within another element|li&gt;a {}|a element directly within an li element|
|Descendant Selector|Applies to elements within another element|p a {}|a elements anywhere inside a p element|
|Adjacent Sibling Selector|Applies to element that immediately follows the other element|h1+p {}|p element just after an h1 element|
|General Sibling Selector|Applies to elements that are a sibling of another element|h1~p {}|All p elements that are siblings of an h1 element|

###Chapter 11

1) 5 ways to define color: RGB values (&amp; RBGA), Hex codes, Color names &amp; HSL (&amp; HSLA).

2) RGB values are written as: rgb(X,Y,Z). There is also rbga(X,Y,Z,A) where A designates the opacity.

3) Hex codes are written as a hashtag follow but 6 hexadecimal digits: #f92baa. First 2 digits are red, middle 2 are green, last 2 are blue.

4) HSL stand for hue saturation lightness, written as hsl(X,Y,Z) where X is the color (0-360), Y is the saturation (0-1) and l is the lightness (0%-100%). A in hsla(X,Y,Z,A) is opacity.

4) There are 147 color names that call on preset colors.

###Chapter 12

1) 3 main types of fonts: serif (has extra stroke/details), sans-serif (straight edges, cleaner design), &amp; monospace (every letter has the same width).

2) Font stacks (designating multiple fonts) can be used to create default fonts if the browser does not have the initial fonts installed. Always end a stack with a font type.

3) Try not to use more than 3 different fonts on a page.

4) Font-size can accept pixel sizes (Xpx), percentages (X%), or m-widths (Xem).

5) @font-face allows you to install a font for use on a browser. Example:

@font-face {font-family: 'Name'; src: url(path);}

Where Name is the name you will use to refer to the font and path is the relative file location. format can also be used to specify the format of the font.

6) text-shadow requires 3-4 values: X, Y, Z, C. X is the left/right shift, Y is the up/down shift, Z is the blur (optional), and C is the color. X, Y, &amp; Z can be in px, %, or em.

7) Pseudo-elements &amp; pseudo-classes go outside the brackets and attach to the end of the selector, modifying to what the rules inside apply.

|Attribute Selector|Meaning|Example|Function|
|---|---|---|---|
|Existence|Matches an attribute|p[class]|Targets any p element with a class attribute|
|Equality|Matches an attribute with a specific value|p[class="dog"]|Targets any p element with a class attribute whose value is dog|
|Space|Matches an attribute with the value in a set of space-separated words|p[class~="dog"]|Targets any p element with class attribute that has dog in its value list|
|Prefix|Matches attribute whose value starts with the string|p[attr^"d"]|Targets any p element with an attribute that has a value starting with "d"|
|Substring|Matches attribute whose value contains the string|p[attr*"do"]|Targets any p element whose attribute contains "do"|
|Suffix|Matches attribute whose value ends with the string|p[attr$"g"]|Targets any p element whose attribute ends with "g"|

###Chapter 13

1) For width and height: Using px will fix the dimensions, em will use dimensions relative to text size, and % will use dimensions relative to the page or containing box.

2) Primary use of min-width, min-height, max-width, &amp; max-height is to ensure that browser dimensions do not over-distort your web page.

3) Border is the outline of a box, margin is the spacing outside of the border, and padding is the spacing between the border and the content. border-width: W X Y Z can be used to designate all 4 sides (W=top, X=right, Y=bottom, Z=left). Also works for border-color:.

4) To center a box, set a fixed width and then use auto for margin-left and margin-right. May also have to use text-align outside the box on older browsers.

###Chapter 14

1) Ordered List Styles: decimal, decimal-leading-zero, lower-alpha, upper-alpha, lower-roman, upper-roman.

2) Unordered List Styles: none, disc, circle, square.

3) Tables can use border, margin, and padding properties on individual cells.

4) Options for cursor: include auto, crosshair, default, pointer, move, text, wait, help, &amp; url("URL").

###Chapter 15

1) Normal Flow: Each block-level element appears on a new line, the default behavior. position:static.

2) Relative Positioning: Shifts an element based on its positioning in normal flow, does not affect other blocks. position:relative, then use top:, right:, bottom:, or left: to dictate the offset.

3) Absolute Positioning: Removes block from normal flow and places it relative to the parent box. Other blocks will ignore it, and it will maintain position as user scrolls the page. position:absolute, then use top:, right:, bottom:, or left: to dictate position.

4) Fixed Positioning: Like absolute positioning but relative to the browser window instead. position:fixed.

5) Floating Elements: Removes block from normal flow and aligns to the left or right of the parent box. Other elements will flow around it. float:(side). Use this to place side-by-side elements. If all elements in a box are floating, then add overflow:auto and width:100% to prevent collapse.

6) Layouts should try to be roughly 1000px wide and fit attention grabbing content in top 600px.

7) Fixed Layouts: Use px dimensions to create a layout that does not change with screen size or resolution. Allows great control over site appearance and ensures relative positioning and size will be maintained; however, does not work well if user adjusts text size or has a screen resolution that is outside of its scope.

8) Liquid Layouts: Use % dimensions to create a layout that adapts to screen size/resolution easily. Pages will adapt to be viewable on almost all resolutions and leave very little unintentional white space; however, without min/max dimensions the page may be unreadable for extreme resolutions and fixed-size elements like images may cause issues on small screens.

###Chapter 16

1) Create a standard set of classes each with a specific set of css properties to be re-used as needed.

###Chapter 17

1) Several new elements intended to aid in organization: &lt;header&gt;, &lt;footer&gt;, &lt;nav&gt;, &lt;article&gt;, &lt;aside&gt;, &lt;section&gt;, &amp; &lt;hgroup&gt;. May still use  &lt;div&gt; with class to sort content for use with CSS.

2) Use the following CSS code to enable older browsers to use the new HTML5 tags:

header, section, footer, aside, nav, article, figure {display:block;}

3) The  &lt;a&gt; element can be wrapped around a larger element to turn the entire element into a hyperlink.

###HTML Tags

1) Block elements always start on a new line in the browser.

2) Inline elements start on the same line as the previous element.

|Tag|Purpose/Effect|
|---|---|
|&lt;html&gt;|Use html code, must be in every html file and contain all html formatted information|
|&lt;body&gt;|Show in the main browser window, can only appear once in a file|
|&lt;h1&gt;|Main heading, block element|
|&lt;h2&gt;-&lt;h6&gt;|Sub-headings of various sizes, block element|
|&lt;p&gt;|Paragraph, block element|
|&lt;div&gt;|Creates a block element out of the contents|
|&lt;span&gt;|Creates an inline element out of the contents|
|&lt;head&gt;|Information about the page not shown in the browser|
|&lt;title&gt;|Title of the page shown above URL|
|&lt;b&gt;|Text displays in bold, inline|
|&lt;i&gt;|Text displays in italic, inline|
|&lt;sup&gt;|Text displays as superscript, inline|
|&lt;sub&gt;|Text displays as subscript, inline|
|&lt;br /&gt;|Inserts a line break, empty element|
|&lt;hr /&gt;|Inserts a horizontal rule, empty element|
|&lt;strong&gt;|Shows strong importance, defaults to bold appearance, inline|
|&lt;em&gt;|Shows emphasis, defaults to italic appearance, inline|
|&lt;q&gt;|Denotes a short quotation within a paragraph, adds quotation marks, inline|
|&lt;blockquote&gt;|Denotes a longer quote, creates its own paragraph, block|
|&lt;abbr title=""&gt;|Denotes what an abbreviation means in mouseover text|
|&lt;acronym title=""&gt;|Denotes what an acronym means in mouseover text|
|&lt;cite&gt;|Denotes a reference to another source, appears in italics|
|&lt;dfn&gt;|Denotes that you will be defining the contained term|
|&lt;address&gt;|Denotes contact information for the author of a page|
|&lt;ins&gt;|Denotes content that has been inserted into a document, appears underlined|
|&lt;del&gt;|Denotes content that has been deleted from a document, appears as a strikethrough|
|&lt;s&gt;|Denotes content that is no longer applicable but not deleted, appears as a strikethrough|
|&lt;ol&gt;|Denotes an ordered list, defaults to numbered list, block|
|&lt;ul&gt;|Denotes an unordered list, defaults to bullet points, block|
|&lt;li&gt;|Denotes an item in a list created by &lt;ol&gt; or &lt;ul&gt;, block|
|&lt;dl&gt;|Denotes a list of definitions|
|&lt;dt&gt;|Denotes the term to be defined in the list created by &lt;dl&gt;|
|&lt;dd&gt;|Denotes the definition of the previous term(s) in the list created by &lt;dl&gt;|
|&lt;a&gt;|Creates clickable text|
|&lt;img /&gt;|Used to add an image to a page, empty element, requires use of src and alt attributes|
|&lt;figure&gt;|Used to contain an image and its caption|
|&lt;figcaption&gt;|Used to denote the caption for an image within a figure|
|&lt;table&gt;|Creates a table that will use tr elements|
|&lt;tr&gt;|Denotes a row within a table that uses td elements|
|&lt;td&gt;|Denotes a column within a row|
|&lt;th&gt;|Used like td, but denotes a heading for a row or column|
|&lt;thead&gt;|Used to denote the headings of the table|
|&lt;tbody&gt;|Used to denote the main body of the table|
|&lt;tfoot&gt;|Used to denote the footer of the table|
|&lt;form&gt;|Used to contain form controls, must always use the action attribute|
|&lt;input&gt;|Designates a form control, requires type attribute, empty element, text after element will be visible|
|&lt;textarea&gt;|Specific form control that allows user to enter more text, contained text will be displayed in the input box|
|&lt;select&gt;|Specific form control that creates a drop-down list|
|&lt;option&gt;|Used with &lt;select&gt; to create options for the drop-down menu, contained text will be visible|
|&lt;button&gt;|Creates a button, contained data will display on the button|
|&lt;label&gt;|Parses forms to assist vision-impaired users|
|&lt;fieldset&gt;|Used to group related form controls|
|&lt;legend&gt;|Used inside &lt;fieldset&gt; to create a caption|
|&lt;!DOCTYPE&gt;|Defines which version of html should be used to interpret the document|
|&lt;iframe&gt;|Creates a frame, requires the src, height, and width attributes|
|&lt;meta /&gt;|Used inside &lt;head&gt; to provide information about the page that will not be visible in a browser, empty|
|&lt;script&gt;|Used to run scripts, such as ones made in JavaScript; type denotes script language and src denotes script location|
|&lt;style&gt;|Goes in the &lt;head&gt; element, allows placing of CSS rules inside an html page|

###Attributes

1) Provide additional information about an element, require a name and a value shown as: &lt;tag name="value"&gt;.

2) Global attributes can be used with ANY element.

|Attribute|Value|Purpose/Effect|
|---|---|---|
|href|URL|Used with &lt;a&gt; to create a hyperlink to URL|
|href|mailto: "email address"|Used with &lt;a&gt; to begin composition of an email to the indicated address|
|href|#label|Used with &lt;a&gt; to link to the label in the same document|
|href|URL#label|Used with &lt;a&gt; to link to a label in another document|
|target|_blank|Used with &lt;a&gt; to open a new window|
|id|label|Labels a location in the document, global attribute, label should always start with a letter or underscore|
|src|URL|Used with &lt;img&gt; to indicate location of image file|
|alt|text|Used with &lt;img&gt; to default to text if image cannot be shown|
|title|text|Used with &lt;img&gt; to create mouseover text|
|height|number|Used with &lt;img&gt; to specify height in pixels for the image|
|width|number|Used with &lt;img&gt; to specify width in pixels for the image|
|align|direction|Used with &lt;img&gt; to align the image to the top, bottom, left, right, or middle|
|scope|row/col|Used with &lt;th&gt; to differentiate a row or column heading|
|colspan|number|Used with &lt;th&rt; or &lt;td&rt; to cause an entry to span the number of indicated columns|
|rowspan|number|Used with &lt;th&rt; or &lt;td&rt; to cause an entry to span the number of indicated rows|
|action|URL|Used with &lt;form&gt; to send information collected to the URL|
|method|get/post|Used with &lt;form&gt; to determine how the information is sent to the URL|
|type|format|Used with &lt;input&gt; to determine what type of input is being collected: text/password/radio/checkbox/date/email/url/search allow user to input information, submit/image create a submission button, file allows user to upload a file, hidden creates a hidden form control, submit causes the action to occur when used in a button element|
|name|variable|Used with &lt;input&gt; to identify the input data|
|maxlength|number|Used with &lt;input&gt; to limit the number of characters that can be entered|
|value|name|Used with radio/checkbox/option to create an option with the indicated name, or with submit to label the button|
|checked|checked|Used with radio/checkbox to denote an option selected by default|
|multiple|multiple|Used with &lt;select&gt; allow a user to select multiple options|
|for|id|Used with &lt;label&gt; to associate with the form with matching id|
|required|required|Used in a form control to require user input before submission|
|placeholder|text|Used with a text-type &lt;input&gt; to create placeholder text until user clicks in the text box|
|class|label|Similar to id but can be identical for multiple elements, allows CSS formatting, global attribute|
|seamless|seamless|Removes scrollbars from an iframe|
|content|text|Used after a name attribute to provide context: description="type the description", keywords="list the keywords", robots="nofollow" to remove from search results|
|content|text|Used after a http-equiv attribute to provide context: author="name of author", pragma="no-cache" to prevent caching, expires="date" to set date to stop caching page|

###CSS Properties

####Front properties
|Property|Effect|
|---|---|
|color:|formats text to the indicated color|
|background-color:|formats background of element to the indicated color|
|opacity:|Designates the opacity (scale 0-1) of a color|
|font-family:|Designates a font to be used for text in the element|
|font-size:|Designates a change from the default font size of 16px|
|font-weight:|Designates the weight of the text (normal, bold, etc.)|
|font-style:|Designates the style of the text (normal, italic, oblique)|
|text-transform:|Applies a rule to the text (uppercase, lowercase, capitalize)|
|text decoration:|Decorates the text (none, underline, overline, line-through, blink)|
|line-height:|Designates the height of each line of text, best to use em units|
|letter-spacing:|Designates spacing between letters, best to use em units|
|word-spacing:|Designates spacing between words, best to use em units|
|text-align:|Aligns text horizontally (left, right, center, justify)|
|vertical-align:|Aligns text vertically (baseline, sub, super, top, text-top, middle, bottom, text-bottom)|
|text-indent:|Indents the first line of text in an element, usually in px or em units|
|text-shadow:|Designates a drop-shadow for text|
|width:|Designates the default width of element|
|height:|Designates the default height of an element|
|min-width:|Designates a minimum width for an element|
|min-height:|Designates a minimum height for an element|
|max-width:|Designates a maximum width of an element|
|max-height:|Designates a maximum height of an element|
|overflow:|Denotes what to do with content that does not fit within a box due to width/height properties|
|border-width:|Denotes the width of the border, given in px or thin/medium/thick, can handle TRBL|
|border-(side)-width:|As above but only for the side indicated (top/bottom/left/right)|
|border-style:|Denotes the style for the border (solid, dotted, dashed, double, groove, ridge, inset, outset, or hidden/none)|
|border-color:|Denotes the color of the border, can handle TRBL|
|border-(side)-color|As border-(side)-width but for color|
|border:|Allows denotation of width, style, and color (in that order) with one property|
|padding:|Denotes width of padding in px, %, or em, can handle TRBL or had the side noted with -(side)|
|margin:|Same as above but for margin instead|
|display:|Changes the block type to inline, block, inline-block, or none|
|visibility:|Sets a box to be visible or hidden|
|border-image:|Uses an image for the border; Requires url, slicing locations, and stretch/repeat/round|
|box-shadow:|Same as text-shadow but for the border, add spread to indicate if shadow should go out or in|
|border-radius:|Used to round corners on a border, can handle TRBL, can also use TRBL/TRBL to indicate horizontal/vertical radii for elliptical rounding|
|list-style-type:|Denotes the style of the list, see chapter 14 notes for more details|
|list-style-image:|Uses a url in the format url("URL") to use an image for a bullet point|
|list-style-position:|Denotes position of list markers (outside or inside)|
|list-style:|Allows designation of the marker style, image, and position in any order|
|empty-cells:|In a table, designates how to display empty cells (show, hide, or inherit)|
|border-spacing:|In a table, controls the spacing between cells, horizontal then vertical|
|border-collapse:|In a table, collapse value will cause cells to collapse ignoring spacing, separate will force them to obey spacing rules|
|background-image:|With url("URL") places a background image in the box|
|cursor:|Changes the appearance of the cursor|
|position:|Dictates how a box will be positioned, see Ch15 notes for more details|
|z-index:|Used to determine lay order for elements, higher numbers appear on top of smaller numbers|
|float:|Denotes a floating box, needs a left or right value, should also use width property|
|clear:|No element within the same parent box should touch the indicated side(s); Takes values of left, right, both, or none|
|background-image:|Tessalates the image from url("URL") to fill the entire box as a background|
|background-repeat:|Controls the tessalation of the background, repeat, repeat=x, repeat-y, no-repeat, fixed, &amp; scroll|
|background-position:|Takes 2 values, the horizontal then vertical. can be descriptive, px, or %|
|background:|Shorthand that handles color image repeat attachment position in that order; A missing value will be skipped|

####Back Properties
|Property|Effect|
|---|---|
|rgb(X,Y,Z)|Denotes a color: X=red 0-100, Y=green 0-100, Z=blue 0-100|
|rgba(X,Y,Z,A)|As above but A=opacity 0-1|
|hsl(X,Y,Z)|Denotes a color: X=hue 0-360, Y=saturation 0-1, Z=lightness 0%-100%|
|hsla(X,Y,Z,A)|As above but A=opacity 0-1|
|#XXXXXX|Denotes a color: XXXXXX is a hecadeximal number|
|color name|Denotes a color from a preset|
|font name|specifies the font to be used|
|font type|specifies a type of font, allowing the browser to use the default font of that type|
|font name, font name, font type|A font stack that will default to the first installed font|
|hidden|Used with overflow, hides excess content|
|scroll|Used with overflow, creates a scrollbar to access excess content|

####Pseudo-Elements &amp; Psuedo-Classes
|Name|Effect|
|---|---|
|:first-letter|Applies only to the first letter of the selector|
|:first-line|Applies only to the first line of the selector|
|:link|Applies only to hyperlinks that have not been visited|
|:visited|Applies only to hyperlinks that have been visted|
|:hover|Applies only to hyperlinks that the mouse is hovering over|
|:active|Applies only to hyperlinks that a user is clicking|
|:focus|Applies only to an element with which the user is interacting|

###Escape Characters
|Name|Symbol|Code|
|---|:-:|---|
|Less Than|&lt;|&amp;lt;|
|Greater Than|&gt;|&amp;gt;|
|Ampersand|&amp;|&amp;amp;|
|Quotation Mark|&quot;|&amp;quot;|
|Cent Sign|&cent;|&amp;cent;|
|Pound Sign|&pound;|&amp;pound;|
|Yen Sign|&yen;|&amp;yen;|
|Euro Sign|&euro;|&amp;euro;|
|Copyright Symbol|&copy;|&amp;copy;|
|Registered Trademark|&reg;|&amp;reg;|
|Trademark|&trade;|&amp;trade;|
|Left Single Quote|&lsquo;|&amp;lsquo;|
|Right Single Quote|&rsquo;|&amp;rsquo;|
|Left Double Quote|&ldquo;|&amp;ldquo;|
|Right Double Quote|&rdquo;|&amp;rdquo;|
|Multiplication Sign|&times;|&amp;times;|
|Division Sign|&divide;|&amp;divide;|
