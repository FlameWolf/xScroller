<h1>How to Use</h1>
<ol>
<li>Download <em>xScroller.Minified.zip</em> and extract the files.</li>
<li>Add the following styles and scripts to your page:</li>
<pre>
&lt;link rel=&quot;stylesheet&quot; href=&quot;xScroller.min.css&quot;/&gt;
<span>...</span>
&lt;script type=&quot;text/javascript&quot; src=&quot;jquery-1.11.0.min.js&quot;&gt;&lt;/script&gt;
&lt;script type=&quot;text/javascript&quot; src=&quot;jquery.mousewheel.min.js&quot;&gt;&lt;/script&gt;
&lt;script type=&quot;text/javascript&quot; src=&quot;xScroller.min.js&quot;&gt;&lt;/script&gt;
</pre>
<blockquote>Make sure that you put the files &quot;arrow-down-grey-small.png&quot; and &quot;arrow-up-grey-small.png&quot; in the same folder where &quot;xScroller.min.js&quot; is located.</blockquote>
If IE8 support is needed then add the following:
<br/>
<pre>
&lt;!--[if IE 8]&gt;
&lt;link rel=&quot;stylesheet&quot; href=&quot;xScroller.IE8.min.css&quot;/&gt;
&lt;![endif]--&gt;
</pre>
<blockquote>If you want rounded corners for the scrollbar in IE8 then put the file “PIE.htc” in the same folder as your page.</blockquote>
<li>Invoke xScroller using the following syntax:</li>
<pre>$(&quot;selectorString&quot;).xScroller({
showButtons: false,
	showBesideContent: false,
	updateOnResize: false,
	updateOnContentResize: false
});</pre>
Each of the parameters is explained below:
<blockquote>
<strong>showButtons:</strong> Display scroll buttons.
<br/>
<strong>showBesideContent:</strong> Normally the scrollbar will be positioned on top of the content, so as to not affect the original layout. If this parameter is true, then the scrollbar will decrease the width of the content by the amount of space it takes up.
<br/>
<strong>updateOnResize:</strong> Update the scrollbar if the size of the element it is attached to changes.
<br/>
<strong>updateOnContentResize:</strong> Update the scrollbar if the size of contents of the element it is attached to changes.
</blockquote>
<li>To remove an xScroller scrollbar from an element, invoke xScroller as:</li>
<pre>$(&quot;selectorString&quot;).xScroller(&quot;destroy&quot;);</pre>
</ol>
