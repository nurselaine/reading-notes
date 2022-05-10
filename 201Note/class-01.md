HTML & CSS
I would like to learn more about how to make my webpage more attractive to users and learn more about positioning! (side note: I have the most trouble with positioning!)
Semantic markup: which provides extra information; such as where emphasis is placed in a sentence
<sup> element is used to contain characters that should be superscript such as the suffixes of dates or mathematical concepts like raising a number to a power such as 22 .
<sub> element is used to contain characters that should be subscript. It is commonly used with foot notes or chemical formulas such as H2 0.

HTML Chapter 8: “Extra Markup” (p.176-199)
- Users with older browsers will not be able to view latest features and markups
- Evolution of HTML: HTML 4, XHTML 1.0 which is combo of XML and HTML 4
- DOCTYPE is declared to tell browser which version of HTML is being used
- Comments: <!--[comments go here]-->, may use inline and blocks of mulitple lines
- Attributes 
	- ID attribute: gives element unique identity | is global attribute (can be used on any element)
	- function: Styling and adding functionality to select elements (id="[value]")
	
	- Class attribute: can share value with various elements 
	- function: changes appearance, used with CSS (class="[value]")
Elements
	- Block: will always start on a new line <ul> <p>
	- inline: elements appear adjacent to the previous element <br/> <em><em/>
	- <div>: use to group various elements in a block, useful when styling and organizing
	- <span>: use to group elements inline , helps with styling mulitple inline elements
	- <iframe width:"" height="" src="{link} alt="" ">: creates window in browser for snippit of altnerate page
		- used to add googlemaps | styles {frameborder, seamless scrolling}, always define height & width  
	- <meta>: no closing tag /; communicates with search engines | found in <head>
		- attributes: name with values "description", "keywords", and "robots/noindex/nofollow" to assist with search
Escape Elements
	- <: &lt or &#60
	- >: &gt: or &amp;
	- &: &amp: or &#38;
	- " &ldquo or &#8229 ;" &rdque or &#8221
HTML Chapter 17: “HTML5 Layout” (pp.428-451)
- HTML5 added tags to improve the visibilty and separation of info for web developers
	- <header> Contains essential info like site name 
	- <footer> copyrigt info, privacy, terms & conditions
	- <article> & <section> can have personal header and footer
		- acts as container | similar to <div> | groups related content
	- <nav>: navigation bars allow users to select various pages/sections | use nexted list tags
	- <aside> acts as a container for info related to entire page | nested inside <article? when containing info r/t article section
	- <hgroups>: group together 1+ h1-6 tags
	- <figure> & <figcaption> used to group content(images, videos, diagrams, and other text)
- communicate with older browsers via CSS that new HTML5 elements are block elements (will be inline by default)

HTML Chapter 18: “Process & Design” (pp.452-475)
- Target audience: ask whether product is for individuals or companies 
	- create fictional characters to better understand what potential audience will think
	- Understand motivations for user visitation and udnerstand audience goals