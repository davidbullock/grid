# Grid

Grid - Float method, with flexbox progressive enhancement. No need to add rows. Just a grid parent, grid children, and a modifier class on the parent to control the behaviour of the children nested within.

https://davidbullock.github.io/grid/

or

https://codepen.io/serkai/pen/EoPoEd

## Key take away for grid - don't overthink it

Like Chris Coyier said in this article:
https://css-tricks.com/dont-overthink-it-grids/

As a designer or developer, there are simple requirements to get your layout up and running as soon as possible. It's likely you want a gutter in between your grid columns / children, a gutter in between and all around, or no gutter at all. If you need more support, feel free to add them to your component respectively.

### No need to style the grid

Try to style the component only within the nested grid child, I've added $grid-background-colour for demo purposes - try to work that into your design system respectively.

To modify the behaviour of the grid, add 

Default - no gutter / padding
`o-grid`

Gutter / padding in between grid children / columns only
`o-grid o-grid--pad-off`

Gutter padding all around the the grid children / columns
`o-grid o-grid--pad-off`

Thin line around the grid children / columns
`o-grid o-grid--line`

#### Work with fractions

12 column grid makes sense, and grid supports that. Fractions are even simpler, e.g. "this section element will be two thirds, this aside element will be one third". Easy right? So the classes are based on that to keep things nice and simple. Give the grid child / column a fraction class: 

1/1
`o-grid__col-1-1`

2/3
`o-grid__col-2-3`

1/2
`o-grid__col-1-2`

1/3
`o-grid__col-1-3` 

1/4
`o-grid__col-1-4`

1/5
`o-grid__col-1-5`

1/6
`o-grid__col-1-6`

1/8
`o-grid__col-1-8`

1/12
`o-grid__col-1-12`

##### Flexbox progressive enhancement

Flexbox helps to align the heights of your grid children, as a designer I know that's what I want. For a more flexbox grid solutions checkout the following pens:

https://codepen.io/serkai/pen/dZaWbN

https://codepen.io/serkai/pen/qpbKrE

