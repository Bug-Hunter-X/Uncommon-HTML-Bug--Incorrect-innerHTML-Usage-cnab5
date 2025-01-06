# Uncommon HTML Bug: Incorrect innerHTML Usage

This repository demonstrates an uncommon bug related to the improper use of `innerHTML` in HTML. The bug occurs when directly assigning HTML content to an element using `innerHTML`, potentially leading to unexpected and undesired behavior.

## Bug Description

The primary issue stems from a naive approach to modifying the content of an HTML element, `<div id="myDiv">`,  using `innerHTML`. The code directly assigns new HTML to the `innerHTML` property, but without sanitizing or carefully handling any potential HTML entities, which can easily lead to unexpected results or XSS vulnerabilities.

## Solution

The solution involves using DOM manipulation techniques to add content more securely. This involves creating elements and appending them instead of directly assigning HTML strings. This prevents unexpected behavior and mitigates potential security risks.