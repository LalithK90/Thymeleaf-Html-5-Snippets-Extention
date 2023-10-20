#Thymeleaf Html 5 Snippets
![](https://github.com/LalithK90/Thymeleaf-Html-5-Snippets/blob/main/assets/20230909_131405_image.png)

---

## *What is Thymeleaf ?*

* Thymeleaf is a modern server-side Java template engine for both web and standalone environments, capable of processing HTML, XML, JavaScript, CSS and even plain text.
* The main goal of Thymeleaf is to provide an elegant and highly-maintainable way of creating templates. To achieve this, it builds on the concept of Natural Templates to inject its logic into template files in a way that doesn’t affect the template from being used as a design prototype. This improves communication of design and bridges the gap between design and development teams.
* Thymeleaf has also been designed from the beginning with Web Standards in mind – especially HTML5 – allowing you to create fully validating templates if that is a need for you.

> source([thymeleaf official doc](https://www.thymeleaf.org/doc/tutorials/3.1/usingthymeleaf.pdf))

## Features

---

Thymeleaf code snipptes for "**.html**" files.

#### with **"xmlns"** name space

```thymeleaf initialization
<!DOCTYPE html>
<html xmlns:th="http://www.thymeleaf.org">
  <head>
    <title>Good Thymes Virtual Grocery</title>
    <meta http-equiv="Content-Type" content="text/html; charset=UTF-8" />
  </head>
  <body>
    <p>Welcome to Thymeleaf Html 5 Snippets 😄!</p> 
  </body>
</html>
```


| Trigger         | Context                                                           | Description                                                                                                                                                       |
| ----------------- | ------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `t:text`        | th:text="${variable}"                                             | Display dynamic text in a template.                                                                                                                               |
| `t:utext`       | th:utext="${variable}"                                            | Display dynamic text in a template, while escaping special characters to prevent XSS attacks.                                                                     |
| `t:value`       | th:value="${variable}"                                            | Set the value of an input field, select element, or textarea.                                                                                                     |
| `t:if`          | th:if="${variable}"                                               | Conditionally include or exclude content based on a Boolean expression.                                                                                           |
| `t:unless`      | th:unless="${variable}"                                           | Conditionally exclude content based on a Boolean expression.                                                                                                      |
| `t:each`        | th:each="item : ${item}"                                          | Iterate over a collection of objects and display the data for each one.                                                                                           |
| `t:object`      | th:object="${variable}"                                           | Bind form data to a specific object in the model                                                                                                                  |
| `t:href`        | th:href="@{url}"                                                  | Dynamically set the destination URL for a hyperlink.                                                                                                              |
| `t:src`         | th:src="@{url}"                                                   | Dynamically set the source URL for an image or other media resource.                                                                                              |
| `t:style`       | th:style="${variable} == 'conditional'} ? 'true' : 'false'"       | Set the inline style for an element.                                                                                                                              |
| `t:field`       | th:field="*{name}"                                                | Bind form field values to a specific property of a model object.                                                                                                  |
| `t:action`      | th:action="@{variable}"                                           | Specify the URL for form submissions.                                                                                                                             |
| `t:classappend` | th:classappend="${variable} == 'conditional'} ? 'true' : 'false'" | Specify the URL for form submissions.                                                                                                                             |
| `t:attr`        | th:attr="data-attribute=${variable}"                              | Set arbitrary attributes for an element.                                                                                                                          |
| `t:fragment`    | th:fragment="${content}"                                          | Define a reusable fragment of HTML that can be included in multiple templates.                                                                                    |
| `t:replace`     | th:replace="fragment :: content"                                  | Replace the contents of an element with the contents of a named fragment.                                                                                         |
| `t:include`     | th:include="common-header :: header"                              | Include the contents of another template in the current template.                                                                                                 |
| `t:block`       | th:block="title"                                                  | Define a block of content that can be overridden by templates that extend the current template.                                                                   |
| `t:switch`      | th:switch="${data}"                                               | Conditionally include content based on the value of a variable.                                                                                                   |
| `t:case`        | th:case="anything"                                                | Conjunction with th:switch to define a case in a switch statement.                                                                                                |
| `t:with`        | th:with="anything"                                                | Expose a specific object in the model as a local variable, making it easier to access in the template.                                                            |
| `t:insert`      | th:insert="anything :: anything"                                  | Include the contents of another template in the current template, replacing the contents of an element with an ID that matches the name of the included template. |
| `t:remove`      | th:remove="all"                                                   | Remove an element from the template, including its contents.                                                                                                      |

#### **with **"data"** attribute in html5**

```thymeleaf initialization
<!DOCTYPE html>
<html lang="en">
  <head>
    <title>Good Thymes Virtual Grocery</title>
    <meta http-equiv="Content-Type" content="text/html; charset=UTF-8" />
  </head>
  <body>
    <p>Welcome to Thymeleaf Html 5 Snippets 😄!</p> 
  </body>
</html>
```


| Trigger         | Context                                                                | Description                                                                                                                                                       |
| ----------------- | ------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `dttext`        | data-th-text="${variable}"                                             | Display dynamic text in a template.                                                                                                                               |
| `dtutext`       | data-th-utext="${variable}"                                            | Display dynamic text in a template, while escaping special characters to prevent XSS attacks.                                                                     |
| `dtvalue`       | data-th-value="${variable}"                                            | Set the value of an input field, select element, or textarea.                                                                                                     |
| `dtif`          | data-th-if="${variable}"                                               | Conditionally include or exclude content based on a Boolean expression.                                                                                           |
| `dtunless`      | data-th-unless="${variable}"                                           | Conditionally exclude content based on a Boolean expression.                                                                                                      |
| `dteach`        | data-th-each="item : ${item}"                                          | Iterate over a collection of objects and display the data for each one.                                                                                           |
| `dtobject`      | data-th-object="${variable}"                                           | Bind form data to a specific object in the model                                                                                                                  |
| `dthref`        | data-th-href="@{url}"                                                  | Dynamically set the destination URL for a hyperlink.                                                                                                              |
| `dtsrc`         | data-th-src="@{url}"                                                   | Dynamically set the source URL for an image or other media resource.                                                                                              |
| `dtstyle`       | data-th-style="${variable} == 'conditional'} ? 'true' : 'false'"       | Set the inline style for an element.                                                                                                                              |
| `dtfield`       | data-th-field="*{name}"                                                | Bind form field values to a specific property of a model object.                                                                                                  |
| `dtaction`      | data-th-action="@{variable}"                                           | Specify the URL for form submissions.                                                                                                                             |
| `dtclassappend` | data-th-classappend="${variable} == 'conditional'} ? 'true' : 'false'" | Specify the URL for form submissions.                                                                                                                             |
| `dtattr`        | data-th-attr="data-attribute=${variable}"                              | Set arbitrary attributes for an element.                                                                                                                          |
| `dtfragment`    | data-th-fragment="${content}"                                          | Define a reusable fragment of HTML that can be included in multiple templates.                                                                                    |
| `dtreplace`     | data-th-replace="fragment :: content"                                  | Replace the contents of an element with the contents of a named fragment.                                                                                         |
| `dtinclude`     | data-th-include="common-header :: header"                              | Include the contents of another template in the current template.                                                                                                 |
| `dtblock`       | data-th-block="title"                                                  | Define a block of content that can be overridden by templates that extend the current template.                                                                   |
| `dtswitch`      | data-th-switch="${data}"                                               | Conditionally include content based on the value of a variable.                                                                                                   |
| `dtcase`        | data-th-case="anything"                                                | Conjunction with th:switch to define a case in a switch statement.                                                                                                |
| `dtwith`        | data-th-with="anything"                                                | Expose a specific object in the model as a local variable, making it easier to access in the template.                                                            |
| `dtinsert`      | data-th-insert="anything :: anything"                                  | Include the contents of another template in the current template, replacing the contents of an element with an ID that matches the name of the included template. |
| `dtremove`      | data-th-remove="all"                                                   | Remove an element from the template, including its contents.                                                                                                      |

## Release Notes

---


| Changes descriptions     | Version No.                             |
| :------------------------- | ----------------------------------------- |
| *New Tag was added 🎉️* | 0.1.4<br />0.1.5<br />0.1.6 <br />0.1.7 |
| *Bug fix 🎉️*           | 0.1.2<br />0.1.3                        |


### Version : 0.1.1 🎉️

Initial release of extension

## Get touch with me

---

If there is some things to upgrade or some thing change this extention. Please initialize issue on [**GitHub**](https://github.com/LalithK90/Thymeleaf-Html-5-Snippets/).

[**GitHub**](https://github.com/LalithK90/Thymeleaf-Html-5-Snippets/)

**Enjoy!**     😄
