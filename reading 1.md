# Responsive Web Design

### Mobile Internet usage is growing rapidly and now we need to build websites suitable for all users. The industry response to this question has become responsive web design.

##### Responsive web design: the practice of building a website suitable to work on every device and every screen size, no matter how large or small, mobile or desktop.

### Responsive vs. Adaptive vs. Mobile

##### Responsive: generally means to react quickly and positively to any change.

##### Adaptive: means to be easily modified for a new purpose or situation, such as change.

##### Responsive design websites continually and fluidly change based on different factors, such as viewport width, while adaptive websites are built to a group of preset factors.

##### Mobile: generally means to build a separate website commonly on a new domain solely for mobile users. 

##### Responsive web design is the most popular now, favoring design that dynamically adapts to different browser and device viewports, changing layout and content along the way. 

### Flexible Layouts

##### Responsive web design is broken down into three main components: flexible layouts, media queries, and flexible media.

##### Flexible Layouts: the practice of building the layout of a website with a flexible grid, capable of dynamically resizing to any width.

###### Flexible grids are built using relative length units, most commonly PERCENTAGES or EM units. These relative lengths are then used to declare common grid property values such as width, margin, or padding.

##### Flexible layouts don't like to use fixed measurement units because the viewport height and width continually change from device to device.

##### target ÷ context = result!!!!!!

### Flexible Grid

##### HTML
##### <div class="container">
#####   <section>...</section>
#####  <aside>...</aside>
##### </div>

##### CSS
##### .container {
#####   width: 538px;
##### }
##### section, 
##### aside {
#####  margin: 10px;
##### }
##### section {
#####   float: left;
#####   width: 340px;
##### }
##### aside {
#####   float: right;
#####   width: 158px;
##### }

##### Now, with Flexible Grid:

##### section,
##### aside {
#####   margin: 1.858736059%; /*  10px ÷ 538px = .018587361 */
##### }
##### section {
#####   float: left;
#####   width: 63.197026%;    /* 340px ÷ 538px = .63197026 */   
##### }
##### aside {
#####   float: right;
#####   width: 29.3680297%;  /* 158px ÷ 538px = .293680297 */

##### One can also leverage the min-width, max-width, min-height, and max-height properties for greater control of the webpage.

### Media Queries

##### Media Queries: Provide the ability to specify different styles for individual browser and device circumstances, such as the width of the viewport or device orientation.

##### Multiple ways to use media queries, including using the @media rule inside of an existing style sheet, importing a new style sheet using the @import rule, or by linking to a separate style sheet from within the HTML document.

###### @media is recommended inside of an existing style sheet to avoid unwanted HTTP requests.

##### HTML
##### <!-- Separate CSS File -->
##### <link href="styles.css" rel="stylesheet" media="all and (max-width: 1024px)">

##### CSS
##### /* @media Rule */
##### @media all and (max-width: 1024px) {...}

##### /* @import Rule */
##### @import url(styles.css) all and (max-width: 1024px) {...}

##### Each media query may include a media type followed by one or more expressions. Common media types include all, screen, print, tv, and braille. 

##### The HTML5 specification includes new media types, even including 3d-glasses. 

##### Should a media type not be specified the media query will default the media type to screen.

##### The media query expression that follows the media type may include different media features and values, which then allocate to be true or false.

### Logical Operators in Media Queries

##### 




