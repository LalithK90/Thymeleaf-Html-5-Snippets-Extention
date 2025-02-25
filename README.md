# Thymeleaf Html 5 Snippets
![](https://github.com/LalithK90/Thymeleaf-Html-5-Snippets/blob/main/assets/20230909_131405_image.png)

---

## What is Thymeleaf?

* Thymeleaf is a modern server-side Java template engine for both web and standalone environments, capable of processing HTML, XML, JavaScript, CSS and even plain text.
* The main goal of Thymeleaf is to provide an elegant and highly-maintainable way of creating templates. To achieve this, it builds on the concept of Natural Templates to inject its logic into template files in a way that doesn't affect the template from being used as a design prototype. This improves communication of design and bridges the gap between design and development teams.
* Thymeleaf has also been designed from the beginning with Web Standards in mind – especially HTML5 – allowing you to create fully validating templates if that is a need for you.

> Source: [Thymeleaf Official Doc](https://www.thymeleaf.org/doc/tutorials/3.1/usingthymeleaf.pdf)

## Features

---

Thymeleaf code snippets for "**.html**" files.

### With xmlns namespace

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

| Trigger | Context | Description |
|---------|---------|-------------|
| `t:tmpl` | Basic Thymeleaf HTML template | Thymeleaf HTML template with xmlns namespace |
| `t:text` | th:text="${variable}" | Sets the text content of an element (escapes HTML) |
| `t:utext` | th:utext="${variable}" | Sets unescaped text content (renders HTML as-is) |
| `t:value` | th:value="${variable}" | Specify the initial value for an input element |
| `t:if` | th:if="${condition}" | Renders the element only if the condition is true |
| `t:unless` | th:unless="${condition}" | Renders the element only if the condition is false |
| `t:each` | th:each="item_name : ${list_name}" | Iterates over a collection (like a loop) |
| `t:object` | th:object="${variable}" | Binds a form to a model attribute (e.g., a command object) |
| `t:field` | th:field="*{object_variable_name}" | Binds an input field to a property of the th:object |
| `t:href` | th:href="@{url}" | Dynamically sets the href attribute (URLs) |
| `t:src` | th:src="${variable}" | Specify the URI of an image, iframe, or other embedded resource |
| `t:style` | th:style="${variable}" | Specify inline CSS styles for an element |
| `t:classappend` | th:classappend="${condition} ? 'css_class' : ''" | Appends CSS classes conditionally |
| `t:attr` | th:attr="data-attribute=${variable}" | Set arbitrary attributes for an element |
| `t:fragment` | th:fragment="${fragment_name}" | Defines a reusable template fragment |
| `t:replace` | th:replace="~{fragment_path :: fragment_name}" | Replaces the current element with a fragment |
| `t:include` | th:include="~{fragment_path :: fragment_name}" | Includes a fragment (deprecated in Thymeleaf 3) |
| `t:block` | th:block="${variable_name}" | A non-rendered container for logic (e.g., loops/conditionals) |
| `t:switch` | th:switch="${variable_name}" | Switch-case logic for conditional rendering |
| `t:case` | th:case="value" | Defines a case in a switch statement |
| `t:with` | th:with="variable_name" | Defines local variables for use within the element |
| `t:insert` | th:insert="~{fragment_path :: fragment_name}" | Inserts a fragment into the current element |
| `t:remove` | th:remove="all" | Remove element from output |

### With data attribute in HTML5

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

| Trigger | Context | Description |
|---------|---------|-------------|
| `dt:tmpl` | Basic Thymeleaf HTML template | Thymeleaf HTML template with data attributes |
| `dt:text` | data-th-text="${variable}" | Sets the text content of an element (escapes HTML) |
| `dt:utext` | data-th-utext="${variable}" | Sets unescaped text content (renders HTML as-is) |
| `dt:value` | data-th-value="${variable}" | Specify the initial value for an input element |
| `dt:if` | data-th-if="${condition}" | Renders the element only if the condition is true |
| `dt:unless` | data-th-unless="${condition}" | Renders the element only if the condition is false |
| `dt:each` | data-th-each="item_name : ${list_name}" | Iterates over a collection (like a loop) |
| `dt:object` | data-th-object="${variable}" | Binds a form to a model attribute (e.g., a command object) |
| `dt:field` | data-th-field="*{object_variable_name}" | Binds an input field to a property of the th:object |
| `dt:href` | data-th-href="@{url}" | Dynamically sets the href attribute (URLs) |
| `dt:src` | data-th-src="${variable}" | Specify the URI of an image, iframe, or other embedded resource |
| `dt:style` | data-th-style="${variable}" | Specify inline CSS styles for an element |
| `dt:classappend` | data-th-classappend="${condition} ? 'css_class' : ''" | Appends CSS classes conditionally |
| `dt:attr` | data-th-attr="data-attribute=${variable}" | Set arbitrary attributes for an element |
| `dt:fragment` | data-th-fragment="${fragment_name}" | Defines a reusable template fragment |
| `dt:replace` | data-th-replace="~{fragment_path :: fragment_name}" | Replaces the current element with a fragment |
| `dt:include` | data-th-include="~{fragment_path :: fragment_name}" | Includes a fragment (deprecated in Thymeleaf 3) |
| `dt:block` | data-th-block="${variable_name}" | A non-rendered container for logic (e.g., loops/conditionals) |
| `dt:switch` | data-th-switch="${variable_name}" | Switch-case logic for conditional rendering |
| `dt:case` | data-th-case="value" | Defines a case in a switch statement |
| `dt:with` | data-th-with="variable_name" | Defines local variables for use within the element |
| `dt:insert` | data-th-insert="~{fragment_path :: fragment_name}" | Inserts a fragment into the current element |
| `dt:remove` | data-th-remove="all" | Remove element from output |

## Release Notes

---

| Changes descriptions | Version No. |
|:-------------------|-------------|
| *Existing Tag was modified 🎉️* | 0.1.13<br/>0.1.12<br/>0.1.8 |
| *New Tag was added 🎉️* | 0.1.18<br/>0.1.16<br/>0.1.7<br/>0.1.6<br/>0.1.5<br/>0.1.4 |
| *Bug fix 🎉️* | 0.1.17<br/>0.1.15<br/>0.1.14<br/>0.1.10<br/>0.1.9<br/>0.1.7<br/>0.1.3<br/>0.1.2 |

### Version 0.1.18

Bug fix

## Get in Touch

---

If you find any issues or have suggestions for improvements, please create an issue on [GitHub](https://github.com/LalithK90/Thymeleaf-Html-5-Snippets/).

**Enjoy!** 😄
````
