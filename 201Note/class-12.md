# Class 12 Reading notes

## Read this article on the Chart.js API.
- download Chart.js and use in script tag at top of index 


Chart.js docs: You’ll be needing these!
<a src="https://github.com/chartjs/Chart.js/tree/master/docs">Link to charts<a>

Read the following articles on the Canvas API.

## Basic usage
- canvas: looks like img elements without src or alt: Creates fixed-sized drawing surface that exposes 1+ rendering contexts 
  - Attributes: Width and height (default is 300x150) 
  - Style as any normal image | does not affect draing on canvas 
  - Create canvas environment to display: Script holds function called draw() and excuted once the page is loaded: use load event listener (other options are setTimeout and setInterval)
  - Canvas supports rantangle and paths(Lists of points connected by lines)
  - Make a grid:
    - origin of grid position top left corner 
  - Draw a rectangle:
    - fillRect(x,y,width,height): Draws a filled rectangle
    - strokeRect(x,y,width,height): draws a rectangluar outline
    - clearReact(x,y,width,height): clears spcified rectangle area (transparent)
    - refer back to examples
  - Draw a path:
    - beginPath(Creates new path)
    - Path methods(Set different paths for objects)
    - closePath() adds stright line from current point to starting point
    - stroke() draws the shape by stroking outline
    - fill() fills solid shape
    - arch(x,y,radius,startAngle,endAngle,counterclockwise) center is x,y and starting angle to end angle decides trajectory 
    - quadrativCurveTo(cp1x, cp1y, x, y) and bezierCurveTo(cp1x, cp2y, x, y)
    


Drawing shapes with canvas
Applying styles and colors
Drawing text