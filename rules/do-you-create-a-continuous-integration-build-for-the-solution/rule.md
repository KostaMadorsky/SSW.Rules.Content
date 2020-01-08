---
type: rule
archivedreason: 
title: Do you create a Continuous Integration Build for the Solution?
guid: e4c12ecd-319c-4b6a-94ac-13fde8bdb0df
uri: do-you-create-a-continuous-integration-build-for-the-solution
created: 2013-02-06T18:49:06.0000000Z
authors:
- id: 24
  title: Adam Stephensen
related: []

---

(Before you configure continuous deployment) You need to ensure that the code that you have on the server compiles. A successful CI build without deployment lets you know the solution will compile.

<!--endintro-->
<dl class="image">&lt;dt&gt;
      <img src="ci-build-1.jpg" alt="">
   &lt;/dt&gt;<dd>Figure: The Build definition name should include the project name. The reason for this is that builds for all solutions are placed in the same folder, and including the build name makes the Build Drop folder organised</dd></dl><dl class="image">&lt;dt&gt;
      <img src="ci-build-2.jpg" alt="">
   &lt;/dt&gt;<dd>Figure: On the Trigger tab choose Continuous Integration. This ensures that each check-in results in a build</dd></dl><dl class="image">&lt;dt&gt;
      <img src="ci-build-3.jpg" alt="">
   &lt;/dt&gt;<dd>Figure: On the Workspace tab you need to include all source control folders that are required for the build</dd></dl><dl class="image">&lt;dt&gt;
      <img src="ci-build-4.jpg" alt="">
   &lt;/dt&gt;<dd>Figure: Enter the path to your Drop Folder (where you drop your builds)</dd></dl><dl class="image">&lt;dt&gt;
      <img src="ci-build-5.jpg" alt="">
   &lt;/dt&gt;<dd>Figure: Choose the Default Build template and enter the DeployOnBuild argument to the MSBuild Arguments parameter of the build template</dd></dl><dl class="image">&lt;dt&gt;
      <img src="ci-build-6.jpg" alt="">
   &lt;/dt&gt;<dd>Figure: Queue a build, to ensure our CI build is working correctly</dd></dl><dl class="image">&lt;dt&gt;
      <img src="ci-build-7.jpg" alt="">
   &lt;/dt&gt;<dd>Figure: Before we setup continuous deployment it is important to get a successful basic CI build</dd></dl>