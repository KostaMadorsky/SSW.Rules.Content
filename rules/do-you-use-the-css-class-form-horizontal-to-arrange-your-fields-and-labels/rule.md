---
type: rule
archivedreason: "The class no-longer exists in Bootstrap 4.\nhttps://getbootstrap.com/docs/4.5/components/forms/#form-controls \n\nRelated rule: https://rules.ssw.com.au/how-to-align-your-form-labels"
title: Do you use the CSS class "form horizontal" to arrange your fields and labels?
guid: 5c2ca49f-b126-4f96-a4a0-f3126e91c195
uri: do-you-use-the-css-class-form-horizontal-to-arrange-your-fields-and-labels
created: 2014-09-08T20:59:34.0000000Z
authors:
- id: 38
  title: Drew Robson
related: []

---

You should align labels  **next** to the inputs on medium and large displays and  **above** inputs on small and extra-small displays.

<!--endintro-->

Bootstrap makes this easy. Use the css class  **form-horizontal** on your html form for it to use this behaviour by default.
<dl class="code">&lt;dt&gt; <p>&lt;form class=&quot;form-horizontal&quot;&gt;<br>&#160;&#160;&#160; &lt;div class=&quot;form-group&quot;&gt;<br>&#160;&#160;&#160;&#160;&#160;&#160;&#160; &lt;label for=&quot;inputEmail3&quot; class=&quot;col-sm-2 control-label&quot;&gt;Email&lt;/label&gt;<br>&#160;&#160;&#160;&#160;&#160;&#160;&#160; &lt;div class=&quot;col-sm-10&quot;&gt;<br>&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160; &lt;input type=&quot;email&quot; class=&quot;form-control&quot; id=&quot;inputEmail3&quot; placeholder=&quot;Email&quot;&gt;<br>&#160;&#160;&#160;&#160;&#160;&#160;&#160; &lt;/div&gt;<br>&#160;&#160;&#160; &lt;/div&gt;<br>&#160;&#160;&#160; &lt;div class=&quot;form-group&quot;&gt;<br>&#160;&#160;&#160;&#160;&#160;&#160;&#160; &lt;label for=&quot;inputPassword3&quot; class=&quot;col-sm-2 control-label&quot;&gt;Password&lt;/label&gt;<br>&#160;&#160;&#160;&#160;&#160;&#160;&#160; &lt;div class=&quot;col-sm-10&quot;&gt;<br>&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160;&#160; &lt;input type=&quot;password&quot; class=&quot;form-control&quot; id=&quot;inputPassword3&quot; placeholder=&quot;Password&quot;&gt;<br>&#160;&#160;&#160;&#160;&#160;&#160;&#160; &lt;/div&gt;<br>&#160;&#160;&#160; &lt;/div&gt;<br>&lt;/form&gt;</p>&lt;/dt&gt;<dd>Figure&#58; Example html using Bootstrap to get the above behaviour</dd></dl>
See [http://getbootstrap.com/css/#forms-horizontal](http&#58;//getbootstrap.com/css/#forms-horizontal) for more information.

### Related Rule



* [Do you know how to arrange forms?](/_layouts/15/FIXUPREDIRECT.ASPX?WebId=3dfc0e07-e23a-4cbb-aac2-e778b71166a2&amp;TermSetId=07da3ddf-0924-4cd2-a6d4-a4809ae20160&amp;TermId=8610437d-f6c4-4a62-800b-658c58734875)