
# HTML & CSS Crash Course Tutorial

## HTML & CSS - Introduction
*********************************
- what is html(hypertext markup language)
    - HTML provides the basic structure of sites.
- what is css (cascading style sheet)
    - CSS is used to control presentation, formatting, and layout.
- css used to make web pages with good look.feel look better
- basic tags 
    - !DOCTYPE
    - HTML
    - HEAD
    - BODY
- how to inspect an element


## HTML basic tags 
********************************
- Tags
    - strong tag  - used to represent the important text of a document on the browser.
    - em  - emphasized text
    - small  -  emphasized
    - h1,h2....,h6 - heading tags
    - ul - unordered list(dots,bullets,circle,sqare, etc..)
    - ol - ordered list(numbers,Alphabets,roman letters, etc..)
    - div -  division or a section in an HTML document.(divide pages into sections)
    - hr - drow a horizontal line
    - br - breaking tag for break to next line
    - img - used to add images to the document.(main attributes src,alt)
    - span - an inline container used to mark up a part of a text
    - blockquote - specifies a section that is quoted from another source.
- define styles
- comments - !-- some comments --

## HTML5 semantics
************************************

- semantic tags clearly describes its meaning to both the browser and the developer. 
    - article tag -which makeup an article
    - main tag - for main content
    - section tag - to make certain section
    - aside tag - related to something else
    - header tag - for giving heading
    - footer tag - for giving footer


## HTML forms
********************************
- Tags
    - form - used to create an HTML form for user input
    - label -display instriction texts or texts
       - attributes- name,id,for etc..
       - for attributes helps to findout which element is represented by specific label 
    - input -an input field where the user can enter data
        - main attributes- types,name etc..
        - type attribute -(values - radio,text,password,email,etc ..)
- name attribute is important when using radio type,becouse of it helps group radio inputs


## CSS basics
********************************
- how to use css
- link -a link between a document and an external resource
    - usage -link rel="stylesheet" href="style.css" /
- rel - specify relationship between the two documents.
- href - href attribute specifies the URL of the page the link goes to.
- units of measurements in css - px,em,%,cm,ex,in,am,pc,pt etc..
- text decoration - values(underline,none,line-thorugh)
- font family
- text align 
- line height
- letter spacing
- coloumn-count 
    - for make coloums in the document
- border
    - border-width:--px;
    - border-color:--;
    - border-style:--;
    - we can use them together like border:width style colour;
    - we can specify which border we need to style like - border-bottom
- css comments - /* some texts */
- text-shadow - --px --px colour;
- we can pic colour in hexa codes -(##ffffff for white)
- inline elements - it displayed contents space
    - span,img,strong,em etc..
- block level tags - it need full width space
    - p,div,h1,h2
    - in defaut disply:block
- margin and padding(margin refer outer space of an element padding refer inner space)
- margin become collapse together and bigger value is applied.


## CSS classes and selectors
***********************************************

- classname
- selector
- p.error- p tags only affect error class styles
- we can use mutliple classes like - p.error.name
- we can select items by id -##name
    eg ##name{ we can style here for an element with id name}
- inner selecter - div p{we can style here for p element that inside a div}
- attribute selector - a[href]{we can style here for an a tag have href attribute}
- text-transform - for text transforming
- a[href*="google"] {we can style here for an a tag its href value include text 'google'}
- a[href$-"google"]{we can style here for an a tag its href value end with text 'google'}
    - if it is .pdf then we can easly identify pdf documents
- the cascade- top to bottom
- html elements inherit from parent elements
- inherit- this property helps to inherit properties from parents
    - eg. margin:inherit
- we can ovwrride styles inherited from parent elemets using write its own properties to child elementss


## css layout & position
******************************************

- position
    - values-static,relative,fixed,absolute,sticky
- familier %,em unit measurement
- em inherit parent attribute value and it take as 1 .  (13.21)
    - eg. parent element :10px, child element:1.5 em (15px)
- z-index
    - z index is morethan then forward this element
    - z index is lessthan then backward this element
- padding:--px --px (usage)
- border-radious - helps to change border shape
- white-space
- max-width
- margin 
    -auto keyword automatically adjusted spaces
- box-sizing
- line-height 


## chrome dev tools
*************************************

- delete,edit and hide elements in inpect window
- check and uncheck css styles using inspect window
- save changes using file system
    -> source
    -> filesystem
    -> select file folder
    -> made changes
    -> ctrl+s to save
- familier with inspect headings
    -source,inspctor,network,console etc..
- how to view same webpage into different devices using inspect element.


## Pesudo classes & elements
*********************************************

- psudo classes
- style elements when they are in a particular state
    -hover,focus,first-child,valid,
- outline - reomove outer lines of elements
- all class psudo elements   -11:46
    - ::after
    - ::before
    - ::first-letter
    - ::first-line
    - ::selection


## Media queries
********************************************

- responsive design
- media queries- tell the browser how to an element at particular viewport dimensions
    - max-width and min-width
    - @media screen and(max-width:1000px) means below 1000 px what styles elements have
- viewport meta tag- tell the browser what width the viewport sholud be
    - eg. <meta name="viewport" content="width=device-width,initial-scale=1.0" >
- responsive images - smaller images for mobile device


## video 11 tutorial - next steps
**********************************


## CSS Flexbox
**********************************

1. flexbox help us in fixed heights for columns 
2. does floats properties and clear fixes 
3. Flexbox is a css display type desgined to help us craft CSS layouts much easier 
4. control the positin, size and spacing of elements relative to their parent elements and each other 
5. Flexbox is a new CSS display type that controls position, size and spacing of elements relative to their parrent elements and each other
6. Works great responsively
7. Benifits of Flexbox
    Navigation bars & Menu 
    grid layouts 
    bar charts 
    equal height columns
8. Apply a disply type of flex to the parrent container. Then the children elemets in that container directly becomes flex elements.
9. A flex container expands items to fill available free space or shrinks them to prevent overflow.
10. main axis – The main axis of a flex container is the primary axis along which items are laid out.
11. cross axis – The axis perpendicular to the main axis is called the cross axis.
12. flex-grow is used to expand elements into available space and the rate at which it expands into that available space is governed by the number given. 
   	It is all relative to the other container next to it

   	eg: flex-grow: 1;

13. flex-shrink is just the opposite of flex-grow. It determines the rate at which it gets smaller. 
       higher the value the  more it shrinks.
   
       eg: flex-shrink: 1;

14. flex-wrap prevents elements from going off page when a minimum width is specified

    eg: flex-wrap: wrap;

    "wrap-reverse" helps is reversing the flex items, "no-wrap" values available for flex-wrap

15. Flex-basis - is similar to minimum width. 

    eg: flex-basis: 200px;

    if we apply minimum width to the boxes and shrink the window, scroll bar apperas after a point where minimum width of the screen is less than than applied min width.
    where as if we apply flex-basis the boxes will shrink as normal and no scroll bar will appear.

16. Flex-basis, flex-grow and flex-shrink can be written as one property called flex.
    
    eg: flex 1 0 200px; first number is flex-grow, second is flex shrink, third is flex basis.

17. flex-flow -- control the flow of all the flex elements in the container. can be don as column flow and row flow.
    eg: flex-flow: column;      // The main axis of flex flow is column wise.
        flex 1 0 200px; 	//here the flex basis 200px controls the height of the column.

18. justify content property is only applied to the main axis.
                                      
19. We can use "align-items" is used to align the flex-items in the cross axis flow.

    eg: align-items: center;

20. change the order of th elements in a flex box using order.
    eg.  .one{order: 0;}  // if we change the 0 to 1, this one goes to last.
	 .two{order: 0;}
	 .three{order: 0;}
13. flex-shrink is just the opposite of flex-grow. It determines the rate at which it gets smaller. 
       higher the value the  more it shrinks.
   
       eg: flex-shrink: 1;

14. flex-wrap prevents elements from going off page when a minimum width is specified

    eg: flex-wrap: wrap;

    "wrap-reverse" helps is reversing the flex items, "no-wrap" values available for flex-wrap

15. Flex-basis - is similar to minimum width. 

    eg: flex-basis: 200px;

    if we apply minimum width to the boxes and shrink the window, scroll bar apperas after a point where minimum width of the screen is less than than applied min width.
    where as if we apply flex-basis the boxes will shrink as normal and no scroll bar will appear.

16. Flex-basis, flex-grow and flex-shrink can be written as one property called flex.
    
    eg: flex 1 0 200px; first number is flex-grow, second is flex shrink, third is flex basis.

17. flex-flow -- control the flow of all the flex elements in the container. can be don as column flow and row flow.
    eg: flex-flow: column;      // The main axis of flex flow is column wise.
        flex 1 0 200px; 	//here the flex basis 200px controls the height of the column.

18. justify content property is only applied to the main axis.
                                      
19. We can use "align-items" is used to align the flex-items in the cross axis flow.

    eg: align-items: center;

20. change the order of th elements in a flex box using order.
    eg.  .one{order: 0;}  // if we change the 0 to 1, this one goes to last.
	 .two{order: 0;}
	 .three{order: 0;}


## CSS Animations
**********************************

- Q: How to add backgorund images in CSS ?
   - background-image: url(../img/hero1.jpg);

- Q: How to add color to background image in CSS?
   - background-image: linear-gradient(mention direction how color flow should happen,
   - <color>,
   - <color>,
   - url(../img/hero1.jpg);

- Q: How to crop image in css?
   - backgrounf-postion: <value>; ( if top it crops with top)

- Q: how to crop images in css?
   - clip-path: polygon(x y, x y, x y, x y);
   - x-axis cordinate value 
   - y-axis cordinate value

- Q: how to make a text in center permantely? 
   - use postion absolute and add value for tag : top & left,
   - transform : translate(x , y) - used to move starting postion of the text. (x & y are axis) 

- Q: how to add animations using css?
   - using keyframes method 
   - tage "@keyframes <name>" {
   - 0% (where aninamtion begins) {
   - opacity: __px;
   - transfor: translat/rotate/something else }
   - <anyValue b/w 0% to 100%> { }
   - 100% (where anumations ends) {
   - opacity: __px;
   - transfor: translat/rotate/something else } 

- Q: Animation can be written shorter
	- animation-name:<name> and place it in div/class where animation should happen
	- other tag 
	- animation-duration: <sec>;
	- animation-delay: <deelay sec>;
	- animation-iteration-count: <how many times animation should happen
	- in shorter 
	- animation: <name> <duration> <function>;
