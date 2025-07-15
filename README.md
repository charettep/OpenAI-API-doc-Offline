If you want to generate it yourself, navigate to:

https://platform.openai.com/docs/api-reference/introduction

Press F12 to pop up DevTools

Then CTRL+SHIFT+K (Console tab)

Then copy the following javascript to your clipboard:

```javascript
function expandCollapsedButtons() {
  // Find all collapsed buttons (aria-expanded="false")
  const collapsedButtons = document.querySelectorAll('.param-expand-button.link-style[aria-expanded="false"]');
  
  // Log how many buttons were found
  console.log(`Found ${collapsedButtons.length} collapsed buttons`);
  
  // Click each one to expand it
  collapsedButtons.forEach(button => button.click());
  
  // Return the count so you know if you need to run it again
  return collapsedButtons.length;
}

// Run the function and show how many buttons were expanded
expandCollapsedButtons();
```


Paste it CTRL+V in the console

>> <paste script here>

Run it (press Enter) a couple times (CTRL+V Enter) until the console returns the value 0, meaning there's no more fucking content hidden under expandable buttons

CTRL+P Print as PDF
