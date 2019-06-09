# MOUS Test

## Questions:
**CSS Questions:**
1. **Explain what a mixin is in SASS?**  
A mixin is a block of code that groups CSS declarations that can be re-used, example:
~~~~
@mixin flex() {
  display: -webkit-box;
  display: -moz-box;
  display: -ms-flexbox;
  display: -webkit-flex;
  display: flex;
}

.some-class {
  @include flex;
}
~~~~

2.  **You have two divs one nested inside the other, the parent div has “position: relative" applied to it using css and the child has the property, “position: absolute.” Why might you wrap an absolute positioned element with a relative positioned parent?**  
So that the child divs can be absolutely positioned inside of the parent div, an example can can be seen on the test - the text inside the carousel "Explore Limitless" is absolute positioned inside a div that has the position: relative property.

3.  **In what order does a browser parse a CSS and how does this affect the order in which you write your CSS?**  
Inline -> Style Tags -> CSS file defined in HTML (from top to bottom) -> 2nd CSS File defined in HTML etc.
For example any CSS inside 'mous.css' will overwrite styles in 'slick-theme.min.css', unless it has an `!important` tag.

4.  **What is the "box-sizing” property and how is it commonly used?**  
box-sizing determines the way heights/widths are calculated on the page. `border-box` is commonly used so that both border and padding are included in the width and height of an element.

**JavaScript Questions:**

1.  **Explain what a closure is in JavaScript?**  
A closure is where an inner function has access to the outer (enclosing) functions variables.

2.  **Explain what a promise is in JavaScript?**  
Promises allow you to group commands together and treat their success/failure as a single item.

3.  **Explain what a ternary operator is?**  
The ternary operator takes three arguments. The first is a comparison argument, the second is the result upon a true comparison, and the third is the result upon a false comparison.

4.  **What is the difference between using 2 equals and 3 equals?**  
=== tests for strict equality between two values.
== tests for loose equality and preforms type coercion.

5.  **When would you use forEach?**  
To loop once over an array, example:
```
const cities = ['London', 'Paris', 'Berlin'];

cities.forEach(function(city) {
  console.log(city);
});

//output will be:
London
Paris
Berlin

```

6.  **When would you use map?**  
One example of map would be using it to call a function on each item of an array.


## notes:
Tested on Chrome, Firefox and Edge latest versions, I developed this on a Windows laptop and had no access to a mac this weekend so unable to test Safari.
I optimized the images as the file sizes were very large.