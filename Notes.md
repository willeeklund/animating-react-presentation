Animations in React
===================

## Two types used in Next
* ReactTransitionGroup
* AnimateOnChange

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
  Optional animation when ReactTransitionGroup component was added

### AnimateOnChange
  Function called in render() to determine if a class should be added
  When class is added, perform keyframe-animation
  'animationEnd' event -> remove the class

## Examples
  Animate component
    Show/hide animation
  AnimateOnChange
    keyframe-animation using class

## keyframe-animation with JSS
  Make the keyframes-selector global with the '@'
