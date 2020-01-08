---
type: rule
archivedreason: 
title: Practices - Do you avoid directly modifying the DOM from your components?
guid: 5537a14f-cc51-48fe-828c-b8abc240070f
uri: practices---do-you-avoid-directly-modifying-the-dom-from-your-components
created: 2016-04-22T22:18:30.0000000Z
authors:
- id: 55
  title: Steve Leigh
- id: 72
  title: Gabriel George
related: []

---

Using DOM is fine, but manipulating DOM directly in your component is not. With the introduction of Angular, there has been a big push in ensuring the DOM stays out of your JavaScript code.  It is designed in such a way that an existing Angular application can be ported to another target by simply replacing the template and template loader.  Projects such as [Angular React Native Renderer](http://angularjs.blogspot.com.au/2016/04/angular-2-react-native.html) leverages this to allow native mobile app development in Angular.

<!--endintro-->

* Smaller component code making it easier to maintain
* Faster running and easier to write unit tests
* Easier for designers to get involved


This means that the component's state must expose things that are useful to the template as public properties or fields, and the Angular should read these fields to draw itself.
<dl class="badImage">&lt;dt&gt;<img src="dom1.png" alt="dom1.png"> &lt;/dt&gt;<dd>This component manipulates the DOM directly to show and hide the menu</dd></dl><dl class="goodImage">&lt;dt&gt;<img src="dom2.png" alt="dom2.png">&lt;/dt&gt;<dd>This component sets component state, which the template can use.  It is simpler, more descriptive and easier to test</dd></dl>