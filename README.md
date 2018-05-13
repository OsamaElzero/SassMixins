# Elzero Sass Mixins
A collection of useful SASS Mixins

This Package Include

## Css3 Properties Vendor Prefixer

#### Accept Arguments 

1. Property Name
2. Property Values
3. Vendor Prefixes

#### Example

```
.class {
  @include prefixer(transition, all .3s ease, webkit moz o);
}
 ```

## Opacity

#### Accept Arguments 

1. Property Value

#### Example

`@include opacity(.5);`

## Animation Keyframes

#### Accept Arguments 

1. Animation Name

#### Example

`@include keyframes(SlideUpAndDown);`

## Overlay

#### Accept Arguments 

1. Color

#### Example

`@include overlay(black, .5);`

## Centerer

#### Accept Arguments 

No

#### Example

`@include centerer();`

## Circle

#### Accept Arguments 

1. Animation Name

#### Example

`@include keyframes(SlideUpAndDown)`

## Placeholder

#### Accept Arguments 

1. Animation Name

#### Example

`@include keyframes(SlideUpAndDown)`
