
**HTML:**

\<div>
Some message goes here
\</div>


**CSS:**
```
div {
  width: 100px;
  overflow: hidden;
  white-space: nowrap;
  text-overflow: ellipsis;
}
```
**Live Fiddle** (Please let me know/Raise a PR if this link is not working)
https://jsfiddle.net/mpandit/82u0cL4d/


So, a very simple stuff. Few things to remember:
1. A fix width is required for element (for which you need to restrict the length)
2. The combination of overflow, white-space and text-overflow properties is what it makes possible for this to achieve.

**Additional Info:**

a. white-space may have values of 'nowrap', 'pre', 'normal', 'pre-wrap' and 'pre-line' (This prevents text from wrapping to another line considering width specified)

b. As name suggests, overflow is used when text breaches the width allocated to it

c. text-overflow indicates how the overflowed text that is not displayed should be indicated to user (ellipsis/clip or random text).


**References:**

https://css-tricks.com/almanac/properties/w/whitespace/

https://developer.mozilla.org/en-US/docs/Web/CSS/overflow

https://developer.mozilla.org/en-US/docs/Web/CSS/text-overflow


