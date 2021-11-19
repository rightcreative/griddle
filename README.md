# griddle
<h2>Introducing Griddle - A CSS-Grid Based Grid Framework</h2>

<p>Griddle is a flexible, lightweight grid system that works similarly to grid systems such as Bootstrap or Flex Grid. Unlike these other grid systems however, Griddle is based off of CSS Grid, rather than Flexbox.</p>

<h3>Usage:</h3>

<pre>
  &lt;div class="grid grid12 cg10 rg10"&gt;
      &lt;div class="col s2 e6m"&gt;&lt;/div&gt;
      &lt;div class="col s7m"&gt;&lt;/div&gt;
  &lt;/div&gt;
</pre>
<p><em>This produces a 12-column grid, with two equal-width columns. Columns will stretch to 100% width and stack on mobile, but show side-by-side on medium sized devices and above.</em></p>

<hr/>

<p>To use Griddle, start with a wrapper or parent element with the "grid" class added, as well as a class specifying how many columns you want your grid to have. Grids elements can have anywhere from 1 - 16 columns.</p>

<p>Any child element inside this parent element will represent a "column". Each child element should have a class of <strong>col</strong>, along with classes specifying the start column and end column. By default, child elements will stretch from the first column to the last column, depending on how many columns you specified for your grid. So, if you specified a 16-column grid, child elements would stretch from column 1 to column 16.</p>

<p>Because of the default column stretching, if any column will start at column 1, or end at the last available column, you do not need to included classes specifying that, as seen in the example above.</p>

<p>To specify a start column, use a classname of <strong>s</strong> followed by the column number (ie s1).</p>

<p>To specify an end column, use a class name of <strong>e</strong> followed by the column number (ie e12).</p>

<p>You can also append "breakpoint" classes to the end, to specify different start or end columns on different screen sizes. Options include <strong>xs</strong>, <strong>s</strong>, <strong>m</strong>, <strong>l</strong>, and <strong>xl</strong> (ie s2m e11m).</p>

<p>There are various examples below to demonstrate proper usage of this library.</p>

<p>With Griddle, you can also specify the gap between columns and rows. This is a huge advantage over flexbox based grid systems, as it allows you to mimic grids used in design software identically. To adjust the gaps between columns and rows, you can use cg and rg classes, up to 50px, in increments of 10px (We also have 12px and 15px available). For example, if you wanted a 10px gap, you would use <strong>cg10</strong> and <strong>rg10</strong>.
