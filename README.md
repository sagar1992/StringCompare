StringCompare
=============
<code>StringCompare($compareThisString, $toThisString, $percentage) //in PHP</code><br/>
<code>SC(compareThisString, toThisString, percentage) //in JS</code><br/><br/>
StringCompare is a addon function to compare two string based on percentage matched. It has two operating mode<br/>
<b>1.Word count mode</b><br/>
<p>This mode will be active by default.It will be useful to compare two sentences. <br/>
For example:<br/>
<code>
StringCompare('Hello World','Hello my world',90) // returns true 
</code><Br/>
<code>
StringCompare('Hello Sagar', 'Hello Ryan',90) // returns false <br/>
</code>
</p>
<b>2.Char count mode</b><br/>
<p>
To enable this mode configuration of the StringCompare needs to be changed. This will be useful to compare two words. <br/> 
For example: <br/>
<code>
StringCompare('letters','letter',50) // returns true <br/>
</code>
</p>

Configuration
=============

To change the mode, following has to be done before applying the funtion.<br/>
These are the options available. <br/>
1. wordcount<br/>
2. charcount<br/>

<b>In PHP</b><br/>
<code>
$option = 'charcount';
</code><br/>
<code>
$config['COMPARE_TYPE'] = $option //Comparision will be done in charcount mode <br/>
</code>

<b>In JS</b><br/>
<code>
SC.setoptions({COMPARE_TYPE:'charcount'});
</code>
