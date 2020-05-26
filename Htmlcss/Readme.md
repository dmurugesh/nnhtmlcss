# HTML & CSS Notes

video tutorial 1 - Introduction

* what is html(hypertext markup language). 
   HTML provides the basic structure of sites.
* what is CSS (cascading style sheet)
   CSS is used to control presentation, formatting, and layout.
   CSS used to make web pages with good look.feel look better
* basic tags
   !DOCTYPE
   HTML
   HEAD
   BODY
* how to inspect an element

video tutorial 2 - html basics

Tags
1. <strong> tag - used to represent the important text of a document on the browser.
2. <em> - emphasized text
3. <small> - emphasized
4. <h1,h2....,h6> - heading tags
5. <ul> - unordered list(dots,bullets,circle,sqare, etc..)
6. <ol> - ordered list(numbers,Alphabets,roman letters, etc..)
7. <div> - division or a section in an HTML document.(divide pages into sections)
8. <hr> - drow a horizontal line
9. <br> - breaking tag for break to next line
10. <img> - used to add images to the document.(main attributes src,alt)
11. <span> - an inline container used to mark up a part of a text
12  <blockquote> - specifies a section that is quoted from another source.
14. How to add comments => !-- some comments --


video 3 tutorial - html forms

Tags
1.<form> - used to create an HTML form for user input
2.<label> -display instriction texts or texts
3.<attributes>- name,id,for etc..
   for attributes helps to findout which element is represented by specific label
4. <input> -an input field where the user can enter data
5. main attributes- types,name etc..
   type attribute -(values - radio,text,password,email,etc ..)
   name attribute is important when using radio type,becouse of it helps group radio inputs

video 4 tutorials - css basics

1. how to use css
   link -a link between a document and an external resource
2. usage -link rel="stylesheet" href="style.css" /
3. rel - specify relationship between the two documents.
4. href - href attribute specifies the URL of the page the link goes to.
5. units of measurements in css - px,em,%,cm,ex,in,am,pc,pt etc..
6. text decoration - values(underline,none,line-thorugh)
7. font family
8. text align
9. line height
10.letter spacing
11.coloumn-count
12.for make coloums in the document
13.border
   border-width:--px;
   border-color:--;
   border-style:--;
14.we can use them together like border:width style colour;
15.we can specify which border we need to style like - border-bottom
16.css comments - /* some texts */
17.text-shadow - --px --px colour;
18.we can pic colour in hexa codes -(##ffffff for white)
19.inline elements - it displayed contents space
20.span,img,strong,em etc..
30.block level tags - it need full width space
  .p,div,h1,h2
  in defaut disply:block
14.margin and padding(margin refer outer space of an element padding refer inner space)
15.margin become collapse together and bigger value is applied.

video 5 tutorials - css classes and selectors

1.  classname
2.  selector
3.  p.error- p tags only affect error class styles
4.  we can use mutliple classes like - p.error.name
5.  we can select items by id -##name eg ##name{ we can style here for an element with id name}
6.  inner selecter - div p{we can style here for p element that inside a div}
7.  attribute selector - a[href]{we can style here for an a tag have href attribute}
8.  text-transform - for text transforming
9.  a[href*="google"] {we can style here for an a tag its href value include text 'google'}
10. a[href$-"google"]{we can style here for an a tag its href value end with text 'google'}
11. if it is .pdf then we can easly identify pdf documents
    the cascade- top to bottom
12. html elements inherit from parent elements
13. inherit- this property helps to inherit properties from parents
    eg. margin:inherit
14. we can overwrite styles inherited from parent elemets using write its own properties to child elementss

video 6 tutorial - html5 semantics

1. semantic tags clearly describes its meaning to both the browser and the developer.
2. article tag -which makeup an article
3. main tag - for main content
4. section tag - to make certain section
5. aside tag - related to something else
6. header tag - for giving heading
7. footer tag - for giving footer

video 7 tutorial - chrome dev tools

1. We can delete,edit and hide elements in inpect window
2. check and uncheck css styles using inspect window
3. save changes using file system -> source -> filesystem -> select file folder -> made changes -> ctrl+s to save
4. familier with inspect headings -source,inspctor,network,console etc..
5. how to view same webpage into different devices using inspect element.

video 8 tutorial - css layout & position

1. position
   values-static,relative,fixed,absolute,sticky
   familier %,em unit measurement
   em inherit parent attribute value and it take as 1 . (13.21)
   eg. parent element :10px, child element:1.5 em (15px)
2. z-index
   z index is morethan 1 then forward this element
   z index is lessthan 1 then backward this element
3. padding:--px --px (usage)
4. border-radious - helps to change border shape
5. white-space
6. max-width
7. margin -auto keyword automatically adjusted spaces
8. box-sizing
9. line-height

video 9 tutorial - psudo classes & elements

1. pesudo classes
   style elements when they are in a particular state -hover,focus,first-child,valid,
   outline - reomove outer lines of elements
2. All class psudo elements -11:46
   ::after
   ::before
   ::first-letter
   ::first-line
   ::selection

video 10 tutorial - intro to media queries

1. responsive design
2. media queries- tell the browser how to an element at particular viewport dimensions
3. max-width and min-width we can set min and max width value
4. @media screen and(max-width:1000px) means below 1000 px what styles elements have
5. viewport meta tag- tell the browser what width the viewport sholud be
	eg.responsive images - smaller images for mobile device


CSS Flexbox


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

20. We can change the order of th elements in a flex box using order property.
    order property accepts postive aswell as negative values
    order goes from negative to postive
    eg.  .one{order: value;} 
	 .two{order: value;}
	 .three{order: value;}


CSS Animations

Q: How to add backgorund images in CSS ?
   background-image: url(../img/hero1.jpg);

Q: How to add color to background image in CSS?
   background-image: linear-gradient(mention direction how color flow should happen,
     <color>,
     <color>,
      url(../img/hero1.jpg);

Q: How to crop image in css?
   backgrounf-postion: <value>; ( if top it crops with top)

Q: how to crop images in css?
   clip-path: polygon(x y, x y, x y, x y);
   x-axis cordinate value 
   y-axis cordinate value

Q: how to make a text in center permantely? 
   use postion absolute and add value for tag : top & left,
   transform : translate(x , y) - used to move starting postion of the text. (x & y are axis) 

Q: how to add animations using css?
   using keyframes method 
   tage "@keyframes <name>" {
   0% (where aninamtion begins) {
   opacity: __px;
   transfor: translat/rotate/something else
   }
   <anyValue b/w 0% to 100%> {
   }
   100% (where anumations ends) {
    opacity: __px;
   transfor: translat/rotate/something else
   } 

Q: Animation can be written shorter
	animation-name:<name> and place it in div/class where animation should happen
	other tag 
	animation-duration: <sec>;
	animation-delay: <deelay sec>;
	animation-iteration-count: <how many times animation should happen
	in shorter 
	animation: <name> <duration> <function>;

