This is my second independent project. Thanks **Julia** for design!

Things that I learned and practised with this projects:

1. **BEM Methodology.** Tried to build page layout with BEM
2. **GRID!** This project was mainly devoted to study and practice Css Grid. Templates, minmax, auto-fit, fr and etc.
3. **SCSS!** variables, functions, nesting, imports, mixins.
4. Super cool opening and closing nav bar with only Css checkbox + smooth show/hide animation on a pure CSS.
5. Very cool hamburger with css animation! 
6. More flexbox practice. Left align of footer nav bar with flex-basis on small screen sizes.
7. Float
8. Calc function in css 
```CSS
max-width: 1200px;
width: calc(100vw - 2em); 
/*subtract from full viewport (100vw) 2em. 1 from each side. 
That gives us nice padding from each side of a screen if screen width is less than max-width(1200)*/

font-size: calc(1.5vw + 1.5rem); 
/*1.5vw - max font size, 1.5rem - min font size. 
This gives us nice and smooths responsive font-size. 
It's bigger in a large screen and smaller in a small screen sizes. No media query!*/
```

9. Triangle tooltip on a Reviews section. I just rotate square, but also this can be made by cropping big border.
```css
&::after{
          content: '';
          display: block;
          position: absolute;
          top: -14px;
          left: 75px;
          background: #FFFFFF;
          border-top: 1px solid rgba(0, 0, 0, 0.2);
          border-left: 1px solid rgba(0, 0, 0, 0.2);
          width: 27px;
          height: 27px;
          transform: rotate(45deg);
        }
```
10. Rem and scss function to calculate rem size. All thanks to Anton Bo!
```scss
$root-font-size: 16px; 

@function rem($size) {
  @return $size / $root-font-size * 1rem;
}

html {
  font-size: $root-font-size;
}

.some-block {
  font-size: rem(24px);
}
```

11. Responsive images with srcset and sizes. In the end I didn't use it but now I know how to use it for future projects
