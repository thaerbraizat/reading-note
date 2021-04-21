![css](https://www.freetutorialsplus.com/css-tutorial/images/css-illustration.png)
# CSS
## Transforms
* The transform property accepts a handful of different values. The rotate value provides the ability to rotate an element from 0 to 360 degrees. 
Using a positive value will rotate an element clockwise, and using a negative value will rotate the element counterclockwise.
* Using the **scale** value within the transform property allows you to change the appeared size of an element.
 The default scale value is 1, therefore any value between .99 and .01 makes an element appear smaller while any value greater than or equal to 1.01 makes an element appear larger.
* Using the translateX value will change the position of an element on the horizontal axis while using the translateY value will change the position of an element on the vertical axis.
* skew, is used to distort elements on the horizontal axis, vertical axis, or both. The syntax is very similar to that of the scale and translate values. Using the skewX value distorts an element on the horizontal axis while the skewY value distorts an element on the vertical axis. To distort an element on both axes the skew value is used,
 declaring the x axis value first, followed by a comma, and then the y axis value %p.
* The transform-origin property can accept one or two values. When only one value is specified, that value is used for both the horizontal and vertical axes.
 If two values are specified, the first is used for the horizontal axis and the second is used for the vertical axis.
* Using the perspective value within the transform property works great for transforming one element from a single, unique perspective. When you want to transform a group of elements all with the same perspective, or vanishing point, apply the perspective property to their parent element.
* By using the scaleZ three-dimensional transform elements may be scaled on the z axis. This isn’t extremely exciting when no other three-dimensional transforms are in place, as there is nothing in particular to scale. In the demonstration below the elements are being scaled up and down on the z axis.
* By using the scaleZ three-dimensional transform elements may be scaled on the z axis. This isn’t extremely exciting when no other three-dimensional transforms are in place, as there is nothing in particular to scale. In the demonstration below the elements are being scaled up and down on the z axis.
## Transitions and Animations
* transition to take place, an element must have a change in state, and different styles must be identified for each state. The easiest way for determining styles for different states is by using the :hover, :focus, :active, and :target pseudo-classes.
* The duration in which a transition takes place is set using the transition-duration property. The value of this property can be set using general timing values, including seconds (s) and milliseconds (ms). 
* The delay sets a time value, seconds or milliseconds, that determines how long a transition should be stalled before executing.
* Animations Keyframes
To set multiple points at which an element should undergo a transition, use the @keyframes rule. The @keyframes rule includes the animation name, any animation breakpoints, and the properties intended to be animated.

* Once you have declared the animation-name property on an element, animations behave similarly to transitions. They include a duration, timing function, and delay if desired. To start, animations need a duration declared using the animation-duration property. As with transitions, the duration may be set in seconds or milliseconds.
* The animation-play-state property allows an animation to be played or paused using the running and paused keyword values respectively. When you play a paused animation, it will resume running from its current state rather than starting from the very beginning again.
* The animation-fill-mode property identifies how an element should be styled either before, after, or before and after an animation is run. The animation-fill-mode property accepts four keyword values, including none, forwards, backwards, and both.
### Resource
* [CSS Transforms](https://learn.shayhowe.com/advanced-html-css/css-transforms/)
* [CSS Transitions & Animations](https://learn.shayhowe.com/advanced-html-css/transitions-animations/)
* [8 simple CSS3 transitions that will wow your users](https://www.webdesignerdepot.com/2014/05/8-simple-css3-transitions-that-will-wow-your-users)

