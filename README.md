# **Elzero Sass Mixins**
A collection of useful SASS Mixins

This Package Include

## Css3 Properties Vendor Prefixer

#### Accept Arguments 

1. Property Name
2. Property Values
3. Vendor Prefixes

#### Example

```css
.class {
  @include prefixer(transition, all .3s ease, webkit moz o);
}
 ```
#### Output

```css
.class {
  -webkit-transition: all .3s ease;
  -moz-transition: all .3s ease;
  -o-transition: all .3s ease;
  transition: all .3s ease;
}
 ```

## Opacity

#### Accept Arguments 

1. Property Value

#### Example

```css
.class {
  @include opacity(.5);
}
```

#### Output

```css
.class {
  zoom: 1;
  filter: alpha(opacity=50);
  opacity: 0.5;
}
 ```

## Animation Keyframes

#### Accept Arguments 

1. Animation Name

#### Example

```css
@include keyframes(BigFont) {
  from {
    font-size: 10px;
  }
  to {
    font-size: 20px;
  }
}
```

#### Output

```css
@-webkit-keyframes BigFont {
  from {
    font-size: 10px;
  }
  to {
    font-size: 20px;
  }
}
@-moz-keyframes BigFont {
  from {
    font-size: 10px;
  }
  to {
    font-size: 20px;
  }
}
@keyframes BigFont {
  from {
    font-size: 10px;
  }
  to {
    font-size: 20px;
  }
}
```

## Overlay

#### Accept Arguments 

1. Color
2. Opacity

#### Example

```css
.class {
  @include overlay(black, .5);
}
```

#### Output

```css
.class {
  position: absolute;
  left: 0;
  top: 0;
  width: 100%;
  height: 100%;
  background-color: rgba(0, 0, 0, 0.5);
}
```

## Centerer

#### Accept Arguments 

No

#### Example

```css
.class {
  @include centerer();
}
```

#### Output

```css
.class {
  position: absolute;
  top: 50%;
  left: 50%;
  -webkit-transform: translate(-50%, -50%);
  -moz-transform: translate(-50%, -50%);
  -o-transform: translate(-50%, -50%);
  transform: translate(-50%, -50%);
}
```

## Circle

#### Accept Arguments 

1. Dimensions Width And Height Must Be The Same

#### Example

```css
.class {
  @include circle(100px);
}
```

#### Output

```css
.class {
  width: 100px;
  height: 100px;
  border-radius: 50%;
}
```

## Placeholder

#### Accept Arguments 

No

#### Example

```css
.class {
  @include placeholder {
    color: #EEE;
  }
}
```

#### Output

```css
.class ::-webkit-input-placeholder {
  color: #EEE;
}
.class ::-moz-placeholder {
  color: #EEE;
}
.class :-ms-input-placeholder {
  color: #EEE;
}
.class :-moz-placeholder {
  color: #EEE;
}
```

## Cover

#### Accept Arguments 

No

#### Example

```css
.class {
  @include cover();
}
```

#### Output

```css
.class {
  -webkit-background-size: cover;
  -moz-background-size: cover;
  -o-background-size: cover;
  background-size: cover;
  background-position: center center;
  background-repeat: no-repeat;
}
```
