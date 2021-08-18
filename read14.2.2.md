# HTML & CSS Part 14
![CSS](https://freefrontend.com/assets/img/html-funny-404-pages/HTML-404-Crying-Baby-Page.gif)
## Transforms
CSS3 introduced new methods for positioning and modifying elements. Alternative approaches to size, position, and modify components may now be used to review general layout techniques. The transform property allows for all of these new approaches.

There are two types of transform properties: two-dimensional and three-dimensional. Each of them has its own set of characteristics and values.

### Transform Syntax
The actual syntax for the transform property is quite simple, including the transform property followed by the value. The value specifies the transform type followed by a specific amount inside parentheses.

1. div {
2. -webkit-transform: scale(1.5);
3. -moz-transform: scale(1.5);
4. -o-transform: scale(1.5);
5. transform: scale(1.5);
6. }

### 2D Transforms

On a two-dimensional or three-dimensional plane, elements can be deformed or altered. The x and y axes, often known as the horizontal and vertical axes, are used in two-dimensional transformations. The x, y, and z axes, as well as the z axis, are all used in three-dimensional transformations. These three-dimensional transformations assist define an element's depth as well as its length and breadth. We'll begin by talking about how to transform components on a two-dimensional plane, then move on to three-dimensional transforms.

2D Rotate

The transform property accepts a handful of different values. The rotate value provides the ability to rotate an element from 0 to 360 degrees. Using a positive value will rotate an element clockwise, and using a negative value will rotate the element counterclockwise. The default point of rotation is the center of the element, 50% 50%, both horizontally and vertically. Later we will discuss how you can change this default point of rotation.

- HTML

1. < figure class="box-1">Box 1</ figure>
2. < figure class="box-2">Box 2</ figure>

              
- CSS

1. .box-1 {
2.  transform: rotate(20deg);
3. }
4. .box-2 {
5. transform: rotate(-55deg);
6. }

## Transitions & Animations

The ability to create behaviors for transitions and animations was one of CSS3's innovations. For years, front end developers have been requesting the option to create these interactions using HTML and CSS instead of JavaScript or Flash. Their request has now been granted.

When an element's state changes, such as when it's hovered over, focused on, active, or targeted, you may use CSS3 transitions to modify its appearance and behavior.

### Transitions
As previously stated, a transition must occur when an element changes state, and various styles must be defined for each stage. The :hover, :focus, :active, and :target pseudo-classes make defining styles for different situations a breeze.

Transition-property, transition-duration, transition-timing-function, and transition-delay are the four transition-related qualities in total. The first three are the most common, although not all of them are necessary to construct a transition.

In the example below the box will change its background color over the course of 1 second in a linear fashion.


1. .box {
2. background: #2db34a;
3.  transition-property: background;
4.  transition-duration: 1s;
5.  transition-timing-function: linear;
6. }
7. .box:hover {
8.  background: #ff7b29;
9. }

## 8 SIMPLE CSS3 TRANSITIONS THAT WILL WOW YOUR USERS
CSS3 has opened up a world of possibilities for UX designers, and the greatest part is that the most interesting portions are really simple to implement.

With just a few lines of code, you can create an outstanding transition effect that will thrill your users, improve engagement, and, if utilized correctly, increase conversions. These effects are also hardware-accelerated and a progressive enhancement that you can utilize right now.

Here are eight really easy effects that will bring your UI to life and bring smiles to your users' faces.

The transition attribute is used to regulate all of these effects (save one). We'll create a div in an HTML page to show how these effects work:

< !DOCTYPE html>

< html>

< head>

 < style type="text/css">

</ style>

</ head>

< body>

< div></ div>

</ body>

</ html>

Having done so, set its width and height (so it has dimensions), its background color (so we can see it) and its transition property.

< style type="text/css">

body > div
{

            width:483px;
            height:298px;
            background:#676470;
            transition:all 0.3s ease;

}

</ style>