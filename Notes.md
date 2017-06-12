Animations in React
===================

## Three types used in Next
* ReactTransitionGroup
* AnimateOnChange
* FLIP animations

### ReactTransitionGroup
  Recommended by Facebook
  Similar to ng-animate
  Mount/Unmount hooks
    Add classes
      .myAnimationName-enter
      .myAnimationName-enter-active
      .myAnimationName-leave
      .myAnimationName-leave-active
    Two parts: JS and CSS - must use same timing
      Remove at unmounting after correct time for the animation
  Transitions
    Transition animation with classes
  Optional animation when ReactTransitionGroup component was added, "appear"

### AnimateOnChange
  Function called in render() to determine if a class should be added
  When class is added, perform keyframe-animation
  'animationEnd' event -> remove the class

## Examples
  Animate component
    Show/hide animation
  AnimateOnChange
    keyframe-animation using class
  Flip animation
    react-flip-move, https://medium.com/developers-writing/animating-the-unanimatable-1346a5aab3cd
    http://joshwcomeau.github.io/react-flip-move/examples/#/shuffle?_k=9riba1

## keyframe-animation with JSS
  Make the keyframes-selector global with the '@'

## Expected hickups
When the dynamic changes, such as the Animate component being unmounted, you need to make changes.

One of the challenges is that render() is called multiple times.
