# minimal web application deployment descriptor (web.xml) for a servlet that sorts integers using sort\_integer\_with_java deployable through a tomcat manager.

Just a web.xml file to deploy the servlet in a webapp server to call sort\_integer\_with_java and use it through a web browser.

I test it locally with : http://localhost:8080/sort_integer_with_java_and_servlet_and_webxml/sortIntegers?intsToSort=6,8,3

-- pom.xml <br/>
dependency : sort\_integer\_with_java<br/>

<br/>
-- web.xml<br/>
&lt;servlet&gt;<br/>
&nbsp;&nbsp;&nbsp;&nbsp;&lt;servlet-name&gt;SortIntegers&lt;/servlet-name&gt;<br/>
&nbsp;&nbsp;&nbsp;&nbsp;&lt;servlet-class&gt;sort_integer_with_java_and_servlet.SortIntegersServlet&lt;/servlet-class&gt;<br/>
<br/>
&lt;servlet-mapping&gt;<br/>
&nbsp;&nbsp;&nbsp;&nbsp;&lt;servlet-name&gt;SortIntegers&lt;/servlet-name&gt;<br/>
&nbsp;&nbsp;&nbsp;&nbsp;&lt;url-pattern&gt;/sortIntegers&lt;/url-pattern&gt;<br/>
