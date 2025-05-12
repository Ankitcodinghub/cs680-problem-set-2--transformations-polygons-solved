# cs680-problem-set-2--transformations-polygons-solved
**TO GET THIS SOLUTION VISIT:** [CS680 Problem Set 2- Transformations & Polygons Solved](https://www.ankitcodinghub.com/product/cs680-problem-set-2-transformations-polygons-solved/)


---

📩 **If you need this solution or have special requests:** **Email:** ankitcoding@gmail.com  
📱 **WhatsApp:** +1 419 877 7882  
📄 **Get a quote instantly using this form:** [Ask Homework Questions](https://www.ankitcodinghub.com/services/ask-homework-questions/)

*We deliver fast, professional, and affordable academic help.*

---

<h2>Description</h2>



<div class="kk-star-ratings kksr-auto kksr-align-center kksr-valign-top" data-payload="{&quot;align&quot;:&quot;center&quot;,&quot;id&quot;:&quot;91381&quot;,&quot;slug&quot;:&quot;default&quot;,&quot;valign&quot;:&quot;top&quot;,&quot;ignore&quot;:&quot;&quot;,&quot;reference&quot;:&quot;auto&quot;,&quot;class&quot;:&quot;&quot;,&quot;count&quot;:&quot;1&quot;,&quot;legendonly&quot;:&quot;&quot;,&quot;readonly&quot;:&quot;&quot;,&quot;score&quot;:&quot;5&quot;,&quot;starsonly&quot;:&quot;&quot;,&quot;best&quot;:&quot;5&quot;,&quot;gap&quot;:&quot;4&quot;,&quot;greet&quot;:&quot;Rate this product&quot;,&quot;legend&quot;:&quot;5\/5 - (1 vote)&quot;,&quot;size&quot;:&quot;24&quot;,&quot;title&quot;:&quot;CS680 Problem Set 2- Transformations \u0026amp; Polygons Solved&quot;,&quot;width&quot;:&quot;138&quot;,&quot;_legend&quot;:&quot;{score}\/{best} - ({count} {votes})&quot;,&quot;font_factor&quot;:&quot;1.25&quot;}">

<div class="kksr-stars">

<div class="kksr-stars-inactive">
            <div class="kksr-star" data-star="1" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="2" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="3" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="4" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="5" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>

<div class="kksr-stars-active" style="width: 138px;">
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>
</div>


<div class="kksr-legend" style="font-size: 19.2px;">
            5/5 - (1 vote)    </div>
    </div>
<div class="page" title="Page 1">
<div class="layoutArea">
<div class="column">
CS 680 PSet 2: Transformations &amp; Polygons

Question 1:

Give pseudo-code for an algorithm to determine if the vertices of a polygon are given in

clockwise (CW) or counterclockwise (CCW) order. You may assume that the polygon is simple and non-degenerate; it may be concave or convex. As an example of acceptable detail, here is example pseudo-code for an algorithm that determines if a 2D polygon is concave or convex:

// Algorithm to determine if a polygon is concave or convex // Polygon vertices could be provided in CW or CCW order

// Three sequential vertices may be collinear

Input: v[1], …, v[N] // N polygon vertices

Output: True or False // True if convex, False if concave

<pre>      Vector e1, e2;
      float z;
      int sign_of_sine_theta=0;
</pre>
// compute cross-product between successive edges

// if sign of all the z values are all the same, then convex // loop around polygon, taking cross product at each vertex

<pre>      for (j=1; j&lt;=N; ++j){
           if(j==N)
</pre>
k=1; else

<pre>                k=j+1;
           if(j==1)
</pre>
i=N; else

i=j-1;

<pre>           e1= v[j]-v[i];
           e2= v[k]-v[j];
           z = (e1.x * e2.y) - (e2.x * e1.y);  // z of cross-product
</pre>
<pre>           if(z &lt; 0.0){
                if(sign_of_sine_theta &gt; 0)
</pre>
return False; // sines with different signs else

<pre>                     sign_of_sine_theta = -1;
</pre>
</div>
</div>
<div class="section">
<div class="layoutArea">
<div class="column">
Submission guidelines:

Please prepare your answers neatly written or typed. Submit electronically on Gradescope. If you have prepared hand-written solutions, please still submit online by uploading a scan or photograph. Acceptable formats are .pdf (preferred), .jpg or .png.

</div>
</div>
</div>
<div class="layoutArea">
<div class="column">
} }

</div>
</div>
<div class="layoutArea">
<div class="column">
<pre>}
else if (z &gt; 0.0){
</pre>
<pre>     if(sign_of_sine_theta &lt; 0)
</pre>
<pre>          return False;
          sign_of_sine_theta = 1;
</pre>
</div>
<div class="column">
// sines with different signs

</div>
</div>
<div class="layoutArea">
<div class="column">
else

</div>
</div>
</div>
<div class="page" title="Page 2">
<div class="layoutArea">
<div class="column">
return True;

</div>
</div>
<div class="layoutArea">
<div class="column">
<ol>
<li>a) &nbsp;Main question: Consider the case when the input to the algorithm is a sequence of polygon vertices and a point known to be within the interior of the polygon (inside the polygon, and not on the boundary). To simplify things, you may assume we have a function “segsIntersect(p1, q1, p2, q2)” which will return a boolean telling you whether the line segments from p1 to q1 and p2 to q2 intersect.</li>
<li>b) &nbsp;Extra credit (5 pts): Suppose the point in the interior of the polygon is not provided. Describe a strategy for finding such a point. Pseudocode not required.</li>
<li>c) &nbsp;Extra credit (10 pts): Look up the “shoelace formula” for the area of a polygon. Can you come up with an alternate algorithm based on this formula? Pseudocode needed here.</li>
</ol>
Question 2:

(a) Write a 4 x 4 homogeneous transform matrix M that when applied to a point

𝑝 = (𝑥,𝑦,𝑧,1) yields 𝑝􏰁 = (𝑥􏰁,𝑦􏰁,𝑧􏰁,1) where

𝑥􏰁 = 1 𝑥− 1 𝑧 +𝑎

√2 √2 𝑦􏰁 = 3𝑦+𝑏

𝑧􏰁 = − 1 𝑥 − 1 𝑧 + 𝑐 √2 √2

(b) WhatthreeorfourbasiccomputergraphicstransformsoccurwhenapplyingMtoa3D point? In other words, how can you decompose M into transforms such as scaling, rotation, translation? Give a homogeneous transform matrix for each, and show the order in which they are multiplied.

Question 3:

Derive the shear matrix that would transform the block “h” character on the left to the italic “h” character on the right. Show your answer first with variables, then replace the variables with values for your final answer.

Question 4:

Consider the following unit quaternions

</div>
</div>
</div>
<div class="page" title="Page 3">
<div class="layoutArea">
<div class="column">
𝑞􏰂 = (0,0,1,√3) 22

𝑞􏰃 = (√3,0,−√3,1) 244

<ol>
<li>a) &nbsp;𝑞􏰂 represents a rotation of angle 𝜃􏰂 about a unit vector 𝑢􏰂. What is this angle and vector? (Note: there are several acceptable answers).</li>
<li>b) &nbsp;𝑞􏰃 represents a rotation of angle 𝜃􏰃 about a unit vector 𝑢􏰃. What is this angle and vector? (Note: again, several acceptable answers).</li>
<li>c) &nbsp;Does rotation by 𝑞􏰂 and 𝑞􏰃 commute? Why?</li>
<li>d) &nbsp;Extra credit (5 pts): When do two rotations commute? When do they not? Prove these
statements. (Hint: consider the equation for quaternion multiplication).
</li>
</ol>
Question 5: (680: 15 pts)

.C .C ..

zz

..

Question 6:

Derive a homogeneous transformation matrix that can be used to reflect 3D points about a plane with equation ax + by + cz = d. Your solution should not include the explicit computation of any Euler rotation matrices Rx, Ry, and Rz.

</div>
</div>
<div class="layoutArea">
<div class="column">
Derive a 3D homogeneous transformation matrix to scale along the u-axis with origin C by

</div>
</div>
<div class="layoutArea">
<div class="column">
Su. Your solution should not use trigonometric functions for Rin or Rout, instead use the

</div>
</div>
<div class="layoutArea">
<div class="column">
orthonormal basis vectors as discussed in class.

</div>
</div>
</div>
