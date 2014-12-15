---
layout: page
title: "Bash"
group: topic
description:
# How sub-pages will be linked to this page
topic: bash
# Relative ordering of topics
order: 3
---


# Bash
{:.ui.dividing.header.no_toc}

## Overview

Bash is one of the most commonly used shell scripting languages. It is what's
run every time you open a terminal, ssh into a server, or run a shell script
(unless you've changed it to run a similar program like ksh or zsh).

Bash is an incredibly powerful development tool. It makes automating certain
tasks incredibly easy, saving you time and headaches. A working knowledge of
bash is also a valuable skill when looking for employment in the tech industry.
Interviewers enjoy asking potential candidates questions that test their
knowledge of the shell environment.

All in all, investing a little time into learning the basics of bash is a very
rewarding endeavor.

## Lessons

{% assign pages_sorted = site.pages | sort: 'order' %}
{% for node in pages_sorted %}
{% if node.group == page.topic %}
- [{{ node.title }}]({{ node.url | replace:'index.html','' | prepend: site.baseprefix }})
{% if node.description %}
    - {{ node.description }}
{% endif %}
{% endif %}
{% endfor %}

## Resources

- Regular Expressions
  - [Regular Expressions 101][regex101]
    - Online regular expression visualizer and quick reference
  - [Regular-Expressions.info][regex-info]
    - Start with the [QuickStart][regex-info-qs]
  - [Sed - An Introduction and Tutorial][sed]
    - A very comprehensive but readable introduction to sed

[regex101]: https://regex101.com/
[regex-info]: http://www.regular-expressions.info/
[regex-info-qs]: http://www.regular-expressions.info/quickstart.html
[sed]: http://www.grymoire.com/Unix/Sed.html

## Readings

| Date  | Reading |
| ----  | ------- |
| 10/8  | [Globbing & Ranges][globbing] |
| 10/22 | TODO    |
| 10/29 | TODO    |
| 11/5  | TODO    |
{:.ui.striped.table}

[globbing]: globbing-ranges/