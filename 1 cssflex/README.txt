** LESSON 1.1: CSS GRID **

CSS FLEX

HTML FILE
<div class="parent-div">
	<div class="child-div">e1</div>
	<div class="child-div">e2</div>
	<div class="child-div">e3</div>
</div>

CSS FILE

1. Basic Syntax
.parent-div
{
	display:flex;
	flex-direction: column;
}

When flex-direction: column is used: 

BEFORE:
=============================
   e1   |   e2    |   e3	|
=============================

AFTER: 

========
   e1   |
========
   e2   |
========
   e3   |
========

2. Custom width for each element

.parent-div
{
	display:flex;
	flex-direction: column;
}

.child-div:nth-of-type(1)
{
	width: 50%;
}

.child-div:nth-of-type(2), .child-div:nth-of-type(3)
{
	width: 25%;
}

BEFORE:
=============================
   e1   |   e2    |   e3	|
=============================

AFTER: 
=============================
      e1      |  e2 |  e3	|
=============================


NOTE: 
1. You can nest flex meaning, child elements can have display:flex too. 