# Introduction
>- **Task 3: Set up readme.md with title and short introductions**
>- **Task 4: Write small C program and set up a workflow to run it**
>- **Task 5: Put C code into readme.md, highlight it and get a workflow status badge for it**
>- **Task 6: List all the contributor and their information in readme.md**
>- **Task 7: Promote the pages and add the link into readme.md**
# Code
```c
{% include_relative code.c %}
```
![example workflow](https://github.com/csci3251-2023/project-team-i/actions/workflows/c-cpp.yml/badge.svg)
# Contributors

{% for student in site.stu %}
  - <img src="{{ student.image }}" width="50" height="50"> @{{ student.user }} ({{ student.name }})
    - {{ student.content | markdownify }}
{% endfor %}
---
Last updated: {{ site.time }}
