# CSS Transforms :

The transform property comes in two different settings, two-dimensional and three-dimensional. Each of these come with their own individual properties and values. 

# transform-syntax
The actual syntax for the transform property is quite simple, including the transform property followed by the value. The value specifies the transform type followed by a specific amount inside parentheses.


**EXAMPLE**


    div {
         -webkit-transform: scale(1.5);
         -moz-transform: scale(1.5);
         -o-transform: scale(1.5);
          transform: scale(1.5);
        }


# 2D Transforms
Elements may be distorted, or transformed, on both a two-dimensional plane or a three-dimensional plane. Two-dimensional transforms work on the x and y axes, known as horizontal and vertical axes. Three-dimensional transforms work on both the x and y axes, as well as the z axis. These three-dimensional transforms help define not only the length and width of an element, but also the depth. We’ll start by discussing how to transform elements on a two-dimensional plane, and then work our way into three-dimensional transforms.


## 2D Rotate
The transform property accepts a handful of different values. The rotate value provides the ability to rotate an element from 0 to 360 degrees. Using a positive value will rotate an element clockwise, and using a negative value will rotate the element counterclockwise. The default point of rotation is the center of the element, 50% 50%, both horizontally and vertically. Later we will discuss how you can change this default point of rotation. 

# Transitions & Animations 

CSS Transitions
CSS transitions allows you to change property values smoothly, over a given duration.

 Mouse over the element below to see a CSS transition effect:



# How to Use CSS Transitions?
To create a transition effect, you must specify two things:

the CSS property you want to add an effect to
the duration of the effect

** Example** 

          div {
               width: 100px;
              height: 100px;
              background: red;
               transition: width 2s;
              }


# CSS Animations :

![](https://miro.medium.com/max/1000/0*z-NzK5spBWCM5gp_.jpg)

# What are CSS Animations?
An animation lets an element gradually change from one style to another.

You can change as many CSS properties you want, as many times as you want.

To use CSS animation, you must first specify some keyframes for the animation.

Keyframes hold what styles the element will have at certain times.

** The animation code **


     @keyframes example {
          0%   {background-color: red;}
         25%  {background-color: yellow;}
        50%  {background-color: blue;}
        100% {background-color: green;}
        }

** The element to apply the animation to **

       div {
              width: 100px;
             height: 100px;
              background-color: red;
            animation-name: example;
            animation-duration: 4s;
            }
