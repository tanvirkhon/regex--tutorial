# Understanding Email Regex

## Introduction:

In this tutorial we will look to understand how the email regex works. Regular expressions or regex are powerful tools for pattern matching in strings and extracting information. In this tutorial I will break down a specific regex used to validate email addresses. By the end of this tutorial, you will hopefully have a better understanding of how each component of the email regex works and why it is important.

## Summary:

In this tutorial we will examine the following regex used to validate email addresses:

/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/

This regex makes sure that the email address begins with a sequence of characters, followed by the @ symbol, then a domain name, and finally a domain extension.
