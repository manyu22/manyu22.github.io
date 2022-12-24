---
layout: default
comments: true
categories: [Blog]
tags: [software, documentation, maintenance]
share: true
title: Curious Case of Documentation
emoticon: thought_balloon
description: Software is all about maintenance, each line of code is a liability
show_links: true

---

I remember seeing a snippet of code for the first time in my school computer lab. It felt like Latin to me and I could hardly make sense of anything except for some mathematical operators scattered throughout. The computer lab teacher didn't make it any easier, either. He gave the impression that coding was only for the smartest of minds and created a sense of elitism.

After spending a decade in software engineering, I am glad I don't feel that way anymore. But in reality, many people in various job families can relate to that feeling. Code is intended for humans, not machines, and a computer doesn't care in which language a programmer has written the code as long as it receives its share of 0s and 1s. Don't get me wrong, I am not trivializing the complexity of modern-day software. Even the most experienced programmers can find it daunting to navigate through software of decent scale and age. It's not an easy task to wade through layers of boilerplate code, abstractions, encapsulation, inheritance, overridden API models, etc. Reading code is essentially like traversing a graph of n nodes with `O(n)` complexity, but if you're trying to find a specific business context, it can be as exhausting as `O(n^2)` for a fully connected graph.

![]({{ site.url }}/images/blog_images/curious-case-of-documentation.png){:target="_blank"}

The main point is that although code is intended for all humans, it requires a certain level of expertise and skills to understand and work with it. Even developers and programmers may struggle with code at times, so it is best to leave it to those who have the necessary skills and experience. A well-written code is always accompanied by well-written documentation, and it is important that the documentation always accurately reflects the business logic of the code at any given point in time.

So, why is code documentation so important, and why is it necessary to keep it up to date.

Code documentation is an essential part of the software development process, as it helps to explain the purpose, design, and operation of code to both developers and non-developers. Code documentation serves several key purposes, including:

1. **Clarifying the purpose and operation of code**: Code documentation helps to explain the purpose and operation of code to developers and non-developers alike. It can provide an overview of the code's intended functionality, and can describe how the code fits into the overall system. This can help to improve the readability and understandability of the code, and can make it easier for developers to work with and maintain the code.

2. **Facilitates collaboration and communication**: Code documentation facilitates collaboration/communication within a development team. It can provide context and background information about the code, and can help to ensure that all team members are on the same page about the code's intended functionality and design. This can improve the efficiency and effectiveness of the development process.

3. **Improving the maintainability of code**: Code documentation can help to improve the maintainability of code by providing a reference for developers who are working with the code in the future. It can describe the code's dependencies, assumptions, and constraints, and can provide guidance on how to modify or extend the code. This can save time and effort by reducing the need for developers to reverse engineer the code and can help to prevent errors and regressions.

4. **Improving the developer experience**: Code documentation can also improve the developer experience by providing clear and concise instructions on how to use the code, as well as any relevant warnings or considerations. This can help to ensure that developers/dependent teams are able to effectively utilize the code and can avoid any potential issues.

But how ideal is it to keep the documentation up to date with code? Is it an overhead? To be honest, it is not easy, and even if one programmer or engineer lowers the bar or cuts corners, it can start a chain reaction, and before you know it, your documentation and code can easily diverge. The following diagram depicts some of the scenarios in which the two can easily diverge. Various events encountered during the software development journey and product roadmap can easily become reasons to do so. Check the correlation between your code and documentation is 1 `r(code, documentation) = 1` at project start and how it has peaked towards 0 when there was a new feature launch and change in team.

![]({{ site.url }}/images/blog_images/correlation.png){:target="_blank"}

So, how to solve this? Answer is documentation as code, your need to build mechanisms and processes that your documentation is treated like code, there is similar scrutiniy as for the code, your build fails if a code updates a peice of class but documentation was not updated. Following are some of the ideas which have evolved over last 4-5 years.

1. **Use documentation generators**: There are several tools available that can automatically generate code documentation from comments in the code and other sources. For example, Doxygen is a documentation generators that can create HTML documentation from comments in C++. These tools can save time and effort by automatically creating documentation from existing comments in the code, and can be configured to extract documentation from other sources as well.

2. **Use continuous integration and delivery (CI/CD) tools**: Many CI/CD tools, such as Jenkins, GitHub Actions, and Azure DevOps, have built-in support for automatically generating and publishing code documentation. These tools can be configured to generate documentation whenever code is pushed to a repository or whenever a build or deployment is triggered. This can help to ensure that the documentation is always up to date and easily accessible to developers.

3. **Deploy your documentation, don't save it**: This is inline with previous point, code documentation can have its own  repository and can be deployed with tools like Jekyll. This can enforce the version and format of documentation as your product also journeys through various versions of its own.

4. **Use code review tools**: Some code review tools, such as Gerrit, have built-in support for automatically generating and reviewing code documentation. These tools can be configured to automatically generate documentation from comments in the code and to review the documentation as part of the code review process. This can help to ensure that the documentation is accurate and complete, and can help to identify any gaps in the documentation.

5. **Use automated testing tools**: Some automated testing tools, such as JUnit and PyTest, can generate documentation from test cases. This can help to ensure that the documentation reflects the actual behavior of the code, and can help to identify any discrepancies between the code and the documentation.

Overall, documentation ***should not be an afterthought***. Automating the code documentation process can save time and effort, and it can be the **difference between the long-term sustainability of your codebase and overall product**. It is important to carefully consider the needs and goals of your project and to select the appropriate tools.

---

[back]({{site.url}})
