# Reading Notes 03
<hr>

## Chapter 3: “Lists” 
- **Ordered** : numbered items 
- **Unordered**: bullet points
- **Definition**: set of terms and definitions 
- tags **ol** and **li** or use **dl** and **dt / dd**
- Utilize nested lists

## Chapter 13: “Boxes”
- Box default dimension: will hold it's contents
  - use height and width properties via px, %, ems
  - Percentages: makes size of box relative to window
  - ems: bases size off content within box, provides flexibility of box sizes to fit to size of user screen
    - **min-width, max width**: For pages designed to fit size of user's screen to ensure content are visible
    - **min-height, maz-height & overflow**: if content inside box overlaps, use property - **hidden or scroll**
- Borders, Margins, and Padding: ass space between items on a page
  - Border- width, style color: practice using shorthand border styles
    - border: 3px dotted maroon 
  - Padding: Allows space between content and parent element, padding is added onto specified width of box
  - Margin: controls space between divs and boxes - value is in pixels
    - FYI: If one box sits on top of another margins are collapsed, the larger of the two margins will be used & children elements do not inherit margin properties
- Center Content: set width of box then set L or R margins. Content inside box should have text-align property as well
- Display: transform inline element to block
  - inline-blcok allow block element to flow like inline with retaining block features
- Box-shadow: drop shadow around box & add offset, blur, and spread shadow


From the Duckett JS book:

## Chapter 2: “Basic JavaScript Instructions” 
- declare variable 
  - set equal to [] with/ without items
  - values in arrays can be anything
- Array index starts at 0 but .length method counts at 1

## Chapter 4: “Decisions and Loops” from switch statements 
- if/else statment
- **switch statements**: must provide a default option 
- **Type coercion**: JS converts data types to work dynamically with script
- weak types: JS can change data types while strong types require high specifying
- Strict equality operators **=== !== **
- Short circuit values: processing stops once result returns 
- **Loops** check condition and carry out script until condition met
  - initialization, condition, and update
  - For loops: known amount of times needed to loop through script
  - while: unknown times needed to carry out script
  - do while: carry out script at least once