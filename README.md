# Reactive-Squares-2
Combining the elements of Reactive Squares w/ the Site2 button grid.

The intention of this project was to, one, combine the background effect of the first Reactive Squares with the layout of Site2 and, two, simplify the CSS in comparison to the two previous projects.

The first objective was a success. The second was not. To reduce the amount of images, the background images weren't separated like they were in the original Reactive Squares. This worked, but made the :hover events more difficult since with just CSS it's a bit of a hassle to have parent elements affect child elements. As a result of this choice, it actually probably made the code *more* complicated.

Additionally, I wanted to mask any overflow from the boxes when the user hovers over them, but I wasn't able to do that without nesting each one in a div. This would have fixed the overflow but made it so the parent/child dynamic would be different and thus could use `.parent:hover ~ .child{}` to control hover events.