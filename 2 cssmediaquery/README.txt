** LESSON 1.1: CSS GRID **

CSS GRID

HTML FILE
<div class="main-content">
	<div class="element1">element1</div>
	<div class="element2">e2</div>
	<div class="element3">e3</div>
</div>

CSS FILE

.element1
{
	grid-area: element1; 
}

.element2
{
	grid-area: element2; 
}

.element3
{
	grid-area: element3; 
}


.parent-element
{
	display:grid;
	grid-template-areas:
    'element1 element1 element1'
    'element2 element3 element3'
    'element2 element3 element3';
}

Creates this:
 
=============================
		element1			|
=============================
========= ===================
         |					|
   e2    |		e3			|
         |					|
		 |					|
========= ===================


NOTE: 
1. You can nest grids meaning, child elements can have display:grid too. 