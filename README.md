# chrome-bug
Example of Webfont loading bug in Chrome version 48

***How to reproduce the bug***

1. Go to [kwals.github.io/chrome-bug](kwals.github.io/chrome-bug)

2. Refresh the page _before_ clicking on anything.

3. Click on the text -> `Click here and expect to see text below`


***Expected Behavior***

Text `"Hey there, can you see me?"` should appear between headline and iframe.


***Actual Behavior***

Text is not visible.

See example of bug behavior below;
![text does not load](/reproduce-bug.gif "How to Reproduce the Issue")





___________________________________________


***Bug info for Chromium Team***


_Chrome Version_ : Version 48.0.2564.97 (64-bit)

_URLs (if applicable)_ : https://kwals.github.io/chrome-bug

_Other browsers tested_: Chrome 47, Safari

_Add OK or FAIL, along with the version, after other browsers where you have tested this issue_:

Chrome 47: OK

Firefox: OK

Safari: OK
    
    
    

***_What steps will reproduce the problem?_***


1.Navigate to a page with an iframe. 

  Both page and iframe request the same web font.
  
  Page has content that is `display: hidden` until button is clicked.
  
  
2. Refresh page.



3. Click button to show hidden content.


See example at [kwals.github.io/chrome-bug](kwals.github.io/chrome-bug)


***_What is the expected result?_***

Hidden text should become visible.


***_What happens instead?_***

Hidden text is not visible.

