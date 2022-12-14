---
keywords: fastai
description: Quick launch into Variables, Functions, Arrays, IJavaScript HTML, using Jupyter Notebooks
title: Nicolas JavaScript Tutorial
nb_path: _notebooks/2022-09-26-Javascript.ipynb
layout: notebook
---

<!--
#################################################
### THIS FILE WAS AUTOGENERATED! DO NOT EDIT! ###
#################################################
# file to edit: _notebooks/2022-09-26-Javascript.ipynb
-->

<div class="container" id="notebook-container">
        
<div class="cell border-box-sizing text_cell rendered"><div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<h3 id="console.log-output">console.log output<a class="anchor-link" href="#console.log-output"> </a></h3><p>Output to console using the classic programming introduction using a "Hello, World!" message.</p>
<ul>
<li>The command or function is <mark>console.log()</mark></li>
<li>"Hello, World" is a String literal. This is the referred to as <mark>Static text</mark>, as it does not change.</li>
<li>"Hello, World" is a parameter to the console.log command.</li>
<li>The console.log <mark>command outputs the parameter to the console</mark>, so you can see it in this Jupyter document.</li>
<li>Note, in a Web Application, console.log is used for debugging and is not visible from the browser via HTML.  It is used behind the scenes, when using Inspect-&gt;Console from the browser.</li>
</ul>

</div>
</div>
</div>
    {% raw %}
    
<div class="cell border-box-sizing code_cell rendered">
<div class="input">

<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="n">console</span><span class="o">.</span><span class="n">log</span><span class="p">(</span><span class="s2">&quot;Nicolas&quot;</span><span class="p">);</span>
</pre></div>

    </div>
</div>
</div>

</div>
    {% endraw %}

<div class="cell border-box-sizing text_cell rendered"><div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<h3 id="console.log-output-showing-use-of-variable">console.log output showing use of variable<a class="anchor-link" href="#console.log-output-showing-use-of-variable"> </a></h3><p>This second example is a <mark>sequence of code</mark>, two or more lines forms a sequence.  This example defines a variable, then outputs the msg to terminal.</p>
<ul>
<li>The variable "var msg =" is used to capture the data</li>
<li>The console.log(msg) outputs to console</li>
</ul>

</div>
</div>
</div>
    {% raw %}
    
<div class="cell border-box-sizing code_cell rendered">
<div class="input">

<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="n">function</span> <span class="n">logIt</span><span class="p">(</span><span class="n">output</span><span class="p">)</span> <span class="p">{</span>
    <span class="n">console</span><span class="o">.</span><span class="n">log</span><span class="p">(</span><span class="n">output</span><span class="p">);</span>
<span class="p">}</span>
<span class="n">logIt</span><span class="p">(</span><span class="n">msg</span><span class="p">);</span>
</pre></div>

    </div>
</div>
</div>

</div>
    {% endraw %}

<div class="cell border-box-sizing text_cell rendered"><div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<h3 id="Showing-reuse-of-a-function">Showing reuse of a function<a class="anchor-link" href="#Showing-reuse-of-a-function"> </a></h3><p>Now that a function is defined, it can be called from any of the subsequent cell in the Jupyter notebook.  A function/method, is a process of creating a <mark>procedural abstraction</mark>. This a programming practice to promote reuse versus coding the same thing over and over.</p>
<ul>
<li>First call sends a different string message</li>
<li>Second call sends a number</li>
</ul>

</div>
</div>
</div>
    {% raw %}
    
<div class="cell border-box-sizing code_cell rendered">
<div class="input">

<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="n">console</span><span class="o">.</span><span class="n">log</span><span class="p">(</span><span class="s2">&quot;Reuse of logIT&quot;</span><span class="p">)</span>
<span class="n">logIt</span><span class="p">(</span><span class="s2">&quot;Hello, Students!&quot;</span><span class="p">);</span>
<span class="n">logIt</span><span class="p">(</span><span class="mi">2022</span><span class="p">)</span>
</pre></div>

    </div>
</div>
</div>

</div>
    {% endraw %}

<div class="cell border-box-sizing text_cell rendered"><div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<h3 id="Dynamic-or-Loosely-typed-language-(string,-number)">Dynamic or Loosely typed language (string, number)<a class="anchor-link" href="#Dynamic-or-Loosely-typed-language-(string,-number)"> </a></h3><p><mark>JavaScript is a loosely typed language</mark>, meaning you don't have to specify what type of information will be stored in a variable in advance.  The variable type is determined at runtime.  This is similar to Python and most interpretive languages.  Java which is a compiled language is strongly typed, thus you will see string, integer, double, and object in the source code. In JavaScript, the "typeof" keyword returns the type.</p>

</div>
</div>
</div>
    {% raw %}
    
<div class="cell border-box-sizing code_cell rendered">
<div class="input">

<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="n">function</span> <span class="n">logItType</span><span class="p">(</span><span class="n">output</span><span class="p">)</span> <span class="p">{</span>
    <span class="n">console</span><span class="o">.</span><span class="n">log</span><span class="p">(</span><span class="n">typeof</span> <span class="n">output</span><span class="p">,</span> <span class="s2">&quot;;&quot;</span><span class="p">,</span> <span class="n">output</span><span class="p">);</span>
<span class="p">}</span>
<span class="n">console</span><span class="o">.</span><span class="n">log</span><span class="p">(</span><span class="s2">&quot;Looking at dynamic nature of types in JavaScript&quot;</span><span class="p">)</span>
<span class="n">logItType</span><span class="p">(</span><span class="s2">&quot;hello&quot;</span><span class="p">);</span> <span class="o">//</span> <span class="n">String</span>
<span class="n">logItType</span><span class="p">(</span><span class="mi">2020</span><span class="p">);</span>    <span class="o">//</span> <span class="n">Number</span>
<span class="n">logItType</span><span class="p">([</span><span class="mi">1</span><span class="p">,</span> <span class="mi">2</span><span class="p">,</span> <span class="mi">3</span><span class="p">]);</span>  <span class="o">//</span> <span class="n">Object</span> <span class="ow">is</span> <span class="n">generic</span> <span class="k">for</span> <span class="n">this</span> <span class="n">Array</span><span class="p">,</span> <span class="n">which</span> <span class="n">similar</span> <span class="n">to</span> <span class="n">Python</span> <span class="n">List</span>
</pre></div>

    </div>
</div>
</div>

</div>
    {% endraw %}

<div class="cell border-box-sizing text_cell rendered"><div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<h3 id="Build-a-Person-Function/Class-object-and-JSON">Build a Person Function/Class object and JSON<a class="anchor-link" href="#Build-a-Person-Function/Class-object-and-JSON"> </a></h3><p>JavaScript functions have special properties and syntax is shown in many ways.  In fact, a Class in JavaScript is a special function.  Jupyter Notebooks seems to be more friendly to "function" definitions versus "Class", thus this lesson uses "function" and "prototype" versus "Class".</p>
<ul>
<li><mark>Definition of function allows for a collection of data</mark>, the "function Person" allows programmer to retain name, github id, and class of designation.</li>
<li><mark>Definition of a prototype allow for the definition of a method associated with the function</mark> , the "Person.prototype.toJSON" allows the collection of data to be expressed in a json/string versus JavaScript object.</li>
<li><mark>Instance of a function</mark>, the "var teacher = new Person("Mr M", "jm1021", 1977)" line makes a variable "teacher" which is an object representation of "function Person".</li>
</ul>

</div>
</div>
</div>
    {% raw %}
    
<div class="cell border-box-sizing code_cell rendered">
<div class="input">

<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="o">//</span> <span class="n">define</span> <span class="n">a</span> <span class="n">function</span> <span class="n">to</span> <span class="n">hold</span> <span class="n">data</span> <span class="k">for</span> <span class="n">a</span> <span class="n">Person</span>
<span class="n">function</span> <span class="n">Person</span><span class="p">(</span><span class="n">name</span><span class="p">,</span> <span class="n">ghID</span><span class="p">,</span> <span class="n">classOf</span><span class="p">)</span> <span class="p">{</span>
    <span class="n">this</span><span class="o">.</span><span class="n">name</span> <span class="o">=</span> <span class="n">name</span><span class="p">;</span>
    <span class="n">this</span><span class="o">.</span><span class="n">ghID</span> <span class="o">=</span> <span class="n">ghID</span><span class="p">;</span>
    <span class="n">this</span><span class="o">.</span><span class="n">classOf</span> <span class="o">=</span> <span class="n">classOf</span><span class="p">;</span>
    <span class="n">this</span><span class="o">.</span><span class="n">role</span> <span class="o">=</span> <span class="s2">&quot;&quot;</span><span class="p">;</span>
<span class="p">}</span>

<span class="o">//</span> <span class="n">define</span> <span class="n">a</span> <span class="n">setter</span> <span class="k">for</span> <span class="n">role</span> <span class="ow">in</span> <span class="n">Person</span> <span class="n">data</span>
<span class="n">Person</span><span class="o">.</span><span class="n">prototype</span><span class="o">.</span><span class="n">setRole</span> <span class="o">=</span> <span class="n">function</span><span class="p">(</span><span class="n">role</span><span class="p">)</span> <span class="p">{</span>
    <span class="n">this</span><span class="o">.</span><span class="n">role</span> <span class="o">=</span> <span class="n">role</span><span class="p">;</span>
<span class="p">}</span>

<span class="o">//</span> <span class="n">define</span> <span class="n">a</span> <span class="n">JSON</span> <span class="n">conversion</span> <span class="s2">&quot;method&quot;</span> <span class="n">associated</span> <span class="k">with</span> <span class="n">Person</span>
<span class="n">Person</span><span class="o">.</span><span class="n">prototype</span><span class="o">.</span><span class="n">toJSON</span> <span class="o">=</span> <span class="n">function</span><span class="p">()</span> <span class="p">{</span>
    <span class="n">const</span> <span class="n">obj</span> <span class="o">=</span> <span class="p">{</span><span class="n">name</span><span class="p">:</span> <span class="n">this</span><span class="o">.</span><span class="n">name</span><span class="p">,</span> <span class="n">ghID</span><span class="p">:</span> <span class="n">this</span><span class="o">.</span><span class="n">ghID</span><span class="p">,</span> <span class="n">classOf</span><span class="p">:</span> <span class="n">this</span><span class="o">.</span><span class="n">classOf</span><span class="p">,</span> <span class="n">role</span><span class="p">:</span> <span class="n">this</span><span class="o">.</span><span class="n">role</span><span class="p">};</span>
    <span class="n">const</span> <span class="n">json</span> <span class="o">=</span> <span class="n">JSON</span><span class="o">.</span><span class="n">stringify</span><span class="p">(</span><span class="n">obj</span><span class="p">);</span>
    <span class="k">return</span> <span class="n">json</span><span class="p">;</span>
<span class="p">}</span>

<span class="o">//</span> <span class="n">make</span> <span class="n">a</span> <span class="n">new</span> <span class="n">Person</span> <span class="ow">and</span> <span class="n">assign</span> <span class="n">to</span> <span class="n">variable</span> <span class="n">teacher</span>
<span class="n">var</span> <span class="n">teacher</span> <span class="o">=</span> <span class="n">new</span> <span class="n">Person</span><span class="p">(</span><span class="s2">&quot;Mr M&quot;</span><span class="p">,</span> <span class="s2">&quot;jm1021&quot;</span><span class="p">,</span> <span class="mi">1977</span><span class="p">);</span>
<span class="n">teacher</span><span class="o">.</span><span class="n">setRole</span><span class="p">(</span><span class="s2">&quot;Teacher&quot;</span><span class="p">);</span>

<span class="o">//</span> <span class="n">output</span> <span class="n">of</span> <span class="n">Object</span> <span class="ow">and</span> <span class="n">JSON</span><span class="o">/</span><span class="n">string</span> <span class="n">associated</span> <span class="k">with</span> <span class="n">Teacher</span>
<span class="n">logItType</span><span class="p">(</span><span class="n">teacher</span><span class="p">);</span>  <span class="o">//</span> <span class="nb">object</span> <span class="nb">type</span> <span class="ow">is</span> <span class="n">easy</span> <span class="n">to</span> <span class="n">work</span> <span class="k">with</span> <span class="ow">in</span> <span class="n">JavaScript</span>
<span class="n">logItType</span><span class="p">(</span><span class="n">teacher</span><span class="o">.</span><span class="n">toJSON</span><span class="p">());</span>  <span class="o">//</span> <span class="n">json</span><span class="o">/</span><span class="n">string</span> <span class="ow">is</span> <span class="n">useful</span> <span class="n">when</span> <span class="n">passing</span> <span class="n">data</span> <span class="n">on</span> <span class="n">internet</span>
</pre></div>

    </div>
</div>
</div>

</div>
    {% endraw %}

<div class="cell border-box-sizing text_cell rendered"><div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<h3 id="Build-a-Classroom-Array/List-of-Persons-and-JSON">Build a Classroom Array/List of Persons and JSON<a class="anchor-link" href="#Build-a-Classroom-Array/List-of-Persons-and-JSON"> </a></h3><p>Many key elements are shown again.  New elements include...</p>
<ul>
<li><mark>Building an Array</mark>, "var students" is an array of many persons</li>
<li>Building a Classroom, this show <mark>forEach iteration</mark> through an array and <mark>.push adding</mark> to an array.  These are key concepts in all programming languages.</li>
</ul>

</div>
</div>
</div>
    {% raw %}
    
<div class="cell border-box-sizing code_cell rendered">
<div class="input">

<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="o">//</span> <span class="n">define</span> <span class="n">a</span> <span class="n">student</span> <span class="n">Array</span> <span class="n">of</span> <span class="n">Person</span><span class="p">(</span><span class="n">s</span><span class="p">)</span>
<span class="n">var</span> <span class="n">students</span> <span class="o">=</span> <span class="p">[</span> 
    <span class="n">new</span> <span class="n">Person</span><span class="p">(</span><span class="s2">&quot;Anthony&quot;</span><span class="p">,</span> <span class="s2">&quot;tonyhieu&quot;</span><span class="p">,</span> <span class="mi">2022</span><span class="p">),</span>
    <span class="n">new</span> <span class="n">Person</span><span class="p">(</span><span class="s2">&quot;Bria&quot;</span><span class="p">,</span> <span class="s2">&quot;B-G101&quot;</span><span class="p">,</span> <span class="mi">2023</span><span class="p">),</span>
    <span class="n">new</span> <span class="n">Person</span><span class="p">(</span><span class="s2">&quot;Allie&quot;</span><span class="p">,</span> <span class="s2">&quot;xiaoa0&quot;</span><span class="p">,</span> <span class="mi">2023</span><span class="p">),</span>
    <span class="n">new</span> <span class="n">Person</span><span class="p">(</span><span class="s2">&quot;Tigran&quot;</span><span class="p">,</span> <span class="s2">&quot;Tigran7&quot;</span><span class="p">,</span> <span class="mi">2023</span><span class="p">),</span>
    <span class="n">new</span> <span class="n">Person</span><span class="p">(</span><span class="s2">&quot;Rebecca&quot;</span><span class="p">,</span> <span class="s2">&quot;Rebecca-123&quot;</span><span class="p">,</span> <span class="mi">2023</span><span class="p">),</span>
    <span class="n">new</span> <span class="n">Person</span><span class="p">(</span><span class="s2">&quot;Vidhi&quot;</span><span class="p">,</span> <span class="s2">&quot;unknown&quot;</span><span class="p">,</span> <span class="mi">2024</span><span class="p">)</span>
<span class="p">];</span>

<span class="o">//</span> <span class="n">define</span> <span class="n">a</span> <span class="n">classroom</span> <span class="ow">and</span> <span class="n">build</span> <span class="n">Classroom</span> <span class="n">objects</span> <span class="ow">and</span> <span class="n">json</span>
<span class="n">function</span> <span class="n">Classroom</span><span class="p">(</span><span class="n">teacher</span><span class="p">,</span> <span class="n">students</span><span class="p">){</span> <span class="o">//</span> <span class="mi">1</span> <span class="n">teacher</span><span class="p">,</span> <span class="n">many</span> <span class="n">student</span>
    <span class="o">//</span> <span class="n">start</span> <span class="n">Classroom</span> <span class="k">with</span> <span class="n">Teacher</span>
    <span class="n">teacher</span><span class="o">.</span><span class="n">setRole</span><span class="p">(</span><span class="s2">&quot;Teacher&quot;</span><span class="p">);</span>
    <span class="n">this</span><span class="o">.</span><span class="n">teacher</span> <span class="o">=</span> <span class="n">teacher</span><span class="p">;</span>
    <span class="n">this</span><span class="o">.</span><span class="n">classroom</span> <span class="o">=</span> <span class="p">[</span><span class="n">teacher</span><span class="p">];</span>
    <span class="o">//</span> <span class="n">add</span> <span class="n">each</span> <span class="n">Student</span> <span class="n">to</span> <span class="n">Classroom</span>
    <span class="n">this</span><span class="o">.</span><span class="n">students</span> <span class="o">=</span> <span class="n">students</span><span class="p">;</span>
    <span class="n">this</span><span class="o">.</span><span class="n">students</span><span class="o">.</span><span class="n">forEach</span><span class="p">(</span><span class="n">student</span> <span class="o">=&gt;</span> <span class="p">{</span> <span class="n">student</span><span class="o">.</span><span class="n">setRole</span><span class="p">(</span><span class="s2">&quot;Student&quot;</span><span class="p">);</span> <span class="n">this</span><span class="o">.</span><span class="n">classroom</span><span class="o">.</span><span class="n">push</span><span class="p">(</span><span class="n">student</span><span class="p">);</span> <span class="p">});</span>
    <span class="o">//</span> <span class="n">build</span> <span class="n">json</span><span class="o">/</span><span class="n">string</span> <span class="nb">format</span> <span class="n">of</span> <span class="n">Classroom</span>
    <span class="n">this</span><span class="o">.</span><span class="n">json</span> <span class="o">=</span> <span class="p">[];</span>
    <span class="n">this</span><span class="o">.</span><span class="n">classroom</span><span class="o">.</span><span class="n">forEach</span><span class="p">(</span><span class="n">person</span> <span class="o">=&gt;</span> <span class="n">this</span><span class="o">.</span><span class="n">json</span><span class="o">.</span><span class="n">push</span><span class="p">(</span><span class="n">person</span><span class="o">.</span><span class="n">toJSON</span><span class="p">()));</span>
<span class="p">}</span>

<span class="o">//</span> <span class="n">make</span> <span class="n">a</span> <span class="n">CompSci</span> <span class="n">classroom</span> <span class="kn">from</span> <span class="nn">formerly</span> <span class="n">defined</span> <span class="n">teacher</span> <span class="ow">and</span> <span class="n">students</span>
<span class="n">compsci</span> <span class="o">=</span> <span class="n">new</span> <span class="n">Classroom</span><span class="p">(</span><span class="n">teacher</span><span class="p">,</span> <span class="n">students</span><span class="p">);</span>

<span class="o">//</span> <span class="n">output</span> <span class="n">of</span> <span class="n">Objects</span> <span class="ow">and</span> <span class="n">JSON</span> <span class="ow">in</span> <span class="n">CompSci</span> <span class="n">classroom</span>
<span class="n">logItType</span><span class="p">(</span><span class="n">compsci</span><span class="o">.</span><span class="n">classroom</span><span class="p">);</span>  <span class="o">//</span> <span class="n">constructed</span> <span class="n">classroom</span> <span class="nb">object</span>
<span class="n">logItType</span><span class="p">(</span><span class="n">compsci</span><span class="o">.</span><span class="n">classroom</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span><span class="o">.</span><span class="n">name</span><span class="p">);</span>  <span class="o">//</span> <span class="n">abstract</span> <span class="mi">1</span><span class="n">st</span> <span class="n">objects</span> <span class="n">name</span>
<span class="n">logItType</span><span class="p">(</span><span class="n">compsci</span><span class="o">.</span><span class="n">json</span><span class="p">[</span><span class="mi">0</span><span class="p">]);</span>  <span class="o">//</span> <span class="n">show</span> <span class="n">json</span> <span class="n">conversion</span> <span class="n">of</span> <span class="mi">1</span><span class="n">st</span> <span class="nb">object</span> <span class="n">to</span> <span class="n">string</span>
<span class="n">logItType</span><span class="p">(</span><span class="n">JSON</span><span class="o">.</span><span class="n">parse</span><span class="p">(</span><span class="n">compsci</span><span class="o">.</span><span class="n">json</span><span class="p">[</span><span class="mi">0</span><span class="p">]));</span>  <span class="o">//</span> <span class="n">show</span> <span class="n">JSON</span><span class="o">.</span><span class="n">parse</span> <span class="n">inverse</span> <span class="n">of</span> <span class="n">JSON</span><span class="o">.</span><span class="n">stringify</span>
</pre></div>

    </div>
</div>
</div>

</div>
    {% endraw %}

<div class="cell border-box-sizing text_cell rendered"><div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<h3 id="IJavaScript-and-Table-formatting-using-toHTML-method">IJavaScript and Table formatting using toHTML method<a class="anchor-link" href="#IJavaScript-and-Table-formatting-using-toHTML-method"> </a></h3><p>This example builds a <mark>Classroom method _toHTML</mark> which is passed to the IJavaScript interpreter $$.html which renders output similarly to a real website.</p>
<ul>
<li>JavaScript in the _toHTML method is broken into three parts...<ul>
<li>Style part is building CSS inline formatting</li>
<li>Body part is constructing the Table Rows (tr), Table Headings (th), and Table Data (td).  The table data is obtained from a Classroom object.  The JavaScript for loop allows the construction of a new row of data for each person object in the Array.</li>
<li>Return part creates the HTML fragment for rendering</li>
</ul>
</li>
<li>The last line in the example <mark>$$.html is IJavaScript HTML interpreter</mark> and by passing the parameter of the _toHTML method it obtains HTML to render</li>
</ul>

</div>
</div>
</div>
    {% raw %}
    
<div class="cell border-box-sizing code_cell rendered">
<div class="input">

<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="o">//</span> <span class="n">define</span> <span class="n">an</span> <span class="n">HTML</span> <span class="n">conversion</span> <span class="s2">&quot;method&quot;</span> <span class="n">associated</span> <span class="k">with</span> <span class="n">Group</span>
<span class="n">Group</span><span class="o">.</span><span class="n">prototype</span><span class="o">.</span><span class="n">_toHtml</span> <span class="o">=</span> <span class="n">function</span><span class="p">()</span> <span class="p">{</span>
    <span class="o">//</span> <span class="n">HTML</span> <span class="n">Style</span> <span class="ow">is</span> <span class="n">build</span> <span class="n">using</span> <span class="n">inline</span> <span class="n">structure</span>
    <span class="n">var</span> <span class="n">style</span> <span class="o">=</span> <span class="p">(</span>
      <span class="s2">&quot;display:inline-block;&quot;</span> <span class="o">+</span>
      <span class="s2">&quot;border: 2px solid grey;&quot;</span> <span class="o">+</span>
      <span class="s2">&quot;box-shadow: 0.8em 0.4em 0.4em grey;&quot;</span>
    <span class="p">);</span>
  
    <span class="o">//</span> <span class="n">HTML</span> <span class="n">Body</span> <span class="n">of</span> <span class="n">Table</span> <span class="ow">is</span> <span class="n">build</span> <span class="k">as</span> <span class="n">a</span> <span class="n">series</span> <span class="n">of</span> <span class="n">concatenations</span> <span class="p">(</span><span class="o">+=</span><span class="p">)</span>
    <span class="n">var</span> <span class="n">body</span> <span class="o">=</span> <span class="s2">&quot;&quot;</span><span class="p">;</span>
    <span class="o">//</span> <span class="n">Heading</span> <span class="k">for</span> <span class="n">Array</span> <span class="n">Columns</span>
    <span class="n">body</span> <span class="o">+=</span> <span class="s2">&quot;&lt;tr&gt;&quot;</span><span class="p">;</span>
    <span class="n">body</span> <span class="o">+=</span> <span class="s2">&quot;&lt;th&gt;&lt;mark&gt;&quot;</span> <span class="o">+</span> <span class="s2">&quot;Name&quot;</span> <span class="o">+</span> <span class="s2">&quot;&lt;/mark&gt;&lt;/th&gt;&quot;</span><span class="p">;</span>
    <span class="n">body</span> <span class="o">+=</span> <span class="s2">&quot;&lt;th&gt;&lt;mark&gt;&quot;</span> <span class="o">+</span> <span class="s2">&quot;Age&quot;</span> <span class="o">+</span> <span class="s2">&quot;&lt;/mark&gt;&lt;/th&gt;&quot;</span><span class="p">;</span>
    <span class="n">body</span> <span class="o">+=</span> <span class="s2">&quot;&lt;th&gt;&lt;mark&gt;&quot;</span> <span class="o">+</span> <span class="s2">&quot;classOf&quot;</span> <span class="o">+</span> <span class="s2">&quot;&lt;/mark&gt;&lt;/th&gt;&quot;</span><span class="p">;</span>
    <span class="n">body</span> <span class="o">+=</span> <span class="s2">&quot;&lt;th&gt;&lt;mark&gt;&quot;</span> <span class="o">+</span> <span class="s2">&quot;Role&quot;</span> <span class="o">+</span> <span class="s2">&quot;&lt;/mark&gt;&lt;/th&gt;&quot;</span><span class="p">;</span>
    <span class="n">body</span> <span class="o">+=</span> <span class="s2">&quot;&lt;/tr&gt;&quot;</span><span class="p">;</span>
    <span class="o">//</span> <span class="n">Data</span> <span class="n">of</span> <span class="n">Array</span><span class="p">,</span> <span class="n">iterate</span> <span class="n">through</span> <span class="n">each</span> <span class="n">row</span> <span class="n">of</span> <span class="n">compsci</span><span class="o">.</span><span class="n">group</span> 
    <span class="k">for</span> <span class="p">(</span><span class="n">var</span> <span class="n">row</span> <span class="n">of</span> <span class="n">compsci</span><span class="o">.</span><span class="n">group</span><span class="p">)</span> <span class="p">{</span>
      <span class="o">//</span> <span class="n">tr</span> <span class="k">for</span> <span class="n">each</span> <span class="n">row</span><span class="p">,</span> <span class="n">a</span> <span class="n">new</span> <span class="n">line</span>
      <span class="n">body</span> <span class="o">+=</span> <span class="s2">&quot;&lt;tr&gt;&quot;</span><span class="p">;</span>
      <span class="o">//</span> <span class="n">td</span> <span class="k">for</span> <span class="n">each</span> <span class="n">column</span> <span class="n">of</span> <span class="n">data</span>
      <span class="n">body</span> <span class="o">+=</span> <span class="s2">&quot;&lt;td&gt;&quot;</span> <span class="o">+</span> <span class="n">row</span><span class="o">.</span><span class="n">name</span> <span class="o">+</span> <span class="s2">&quot;&lt;/td&gt;&quot;</span><span class="p">;</span>
      <span class="n">body</span> <span class="o">+=</span> <span class="s2">&quot;&lt;td&gt;&quot;</span> <span class="o">+</span> <span class="n">row</span><span class="o">.</span><span class="n">age</span> <span class="o">+</span> <span class="s2">&quot;&lt;/td&gt;&quot;</span><span class="p">;</span>
      <span class="n">body</span> <span class="o">+=</span> <span class="s2">&quot;&lt;td&gt;&quot;</span> <span class="o">+</span> <span class="n">row</span><span class="o">.</span><span class="n">classOf</span> <span class="o">+</span> <span class="s2">&quot;&lt;/td&gt;&quot;</span><span class="p">;</span>
      <span class="n">body</span> <span class="o">+=</span> <span class="s2">&quot;&lt;td&gt;&quot;</span> <span class="o">+</span> <span class="n">row</span><span class="o">.</span><span class="n">role</span> <span class="o">+</span> <span class="s2">&quot;&lt;/td&gt;&quot;</span><span class="p">;</span>
      <span class="o">//</span> <span class="n">tr</span> <span class="n">to</span> <span class="n">end</span> <span class="n">line</span>
      <span class="n">body</span> <span class="o">+=</span> <span class="s2">&quot;&lt;tr&gt;&quot;</span><span class="p">;</span>
    <span class="p">}</span>
  
     <span class="o">//</span> <span class="n">Build</span> <span class="ow">and</span> <span class="n">HTML</span> <span class="n">fragment</span> <span class="n">of</span> <span class="n">div</span><span class="p">,</span> <span class="n">table</span><span class="p">,</span> <span class="n">table</span> <span class="n">body</span>
    <span class="k">return</span> <span class="p">(</span>
      <span class="s2">&quot;&lt;div style=&#39;&quot;</span> <span class="o">+</span> <span class="n">style</span> <span class="o">+</span> <span class="s2">&quot;&#39;&gt;&quot;</span> <span class="o">+</span>
        <span class="s2">&quot;&lt;table&gt;&quot;</span> <span class="o">+</span>
          <span class="n">body</span> <span class="o">+</span>
        <span class="s2">&quot;&lt;/table&gt;&quot;</span> <span class="o">+</span>
      <span class="s2">&quot;&lt;/div&gt;&quot;</span>
    <span class="p">);</span>
  
  <span class="p">};</span>
  
  <span class="o">//</span> <span class="n">IJavaScript</span> <span class="n">HTML</span> <span class="n">processor</span> <span class="n">receive</span> <span class="n">parameter</span> <span class="n">of</span> <span class="n">defined</span> <span class="n">HTML</span> <span class="n">fragment</span>
  <span class="err">$$</span><span class="o">.</span><span class="n">html</span><span class="p">(</span><span class="n">compsci</span><span class="o">.</span><span class="n">_toHtml</span><span class="p">());</span>
</pre></div>

    </div>
</div>
</div>

</div>
    {% endraw %}

</div>
 

