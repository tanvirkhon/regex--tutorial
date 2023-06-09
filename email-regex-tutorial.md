# Understanding Email Regex

## Introduction:

In this tutorial we will look to understand how the email regex works. Regular expressions or regex are powerful tools for pattern matching in strings and extracting information. In this tutorial I will break down a specific regex used to validate email addresses. By the end of this tutorial, you will hopefully have a better understanding of how each component of the email regex works and why it is important.

## Summary:

In this tutorial we will examine the following regex used to validate email addresses:

/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/

This regex makes sure that the email address begins with a sequence of characters, followed by the @ symbol, then a domain name, and finally a domain extension.

## Table of Contents:

1. [Start and End Anchors](#start-end-anchors)
2. [Local Part](#local-part)
3. [At Symbol](#at-symbol)
4. [Domain](#domain)
5. [Dot](#dot)
6. [Domain Extension](#domain-extension)
7. [Author Information](#author-information)

## Start and End Anchors <a name="start-end-anchors"></a>

The start (`^`) and end (`$`) anchors are very important when using regex. They make sure that the whole string matches the pattern defined in the regex. This will help prevent additional characters from being matched before or after the email address.

## Local Part <a name="local-part"></a>

The local part of the email address is the part before the '@' symbol. In the regex, it is expressed by the `([a-z0-9_\.-]+)`. This part of the regex allows lowercase letters, digits, underscores, periods, and hyphens. The plus sign at the end (`+`) indicates that one or more characters are allowed in the local part.

For example the following email addresses are of valid local parts:

- john.doe
- john_doe123
- john-doe

## The @ Symbol <a name="at-symbol"></a>

The (`@`) symbol is a required part of the email address, separating the local part and the domain name.

## Domain <a name="domain"></a>

The domain name is the part of the email address that comes after the '@' symbol and before the domain extension. In the regex, it is represented by `([\da-z\.-]+)`. This part of the regex allows digits, lowercase letters, periods, and hyphens. The plus sign (`+`) indicates that one or more characters are allowed in the domain.

For example the following email addresses are of valid domains:

- john.doe@example
- john_doe123@my-domain

## Dot <a name="dot"></a>

The dot (`.`) is used to separate the domain and the domain extension. In the regex, it is represented by the '.' character.

## Domain Extension <a name="domain-extension"></a>

The domain extension is the part of the email address that comes after the domain and is separated by a dot. In the regex, it is represented by `([a-z\.]{2,6})`. This part of the regex allows lowercase letters and periods. The curly braces `{2,6}` indicate that the domain extension must have a length between 2 and 6 characters.

Examples of valid domain extensions:

- .com
- .org
- .net

## Author Information <a name="author-information"></a>

This tutorial was created by me Tanvir Khondakar. I am currently a student at the University of Minnesota Bootcamp. If you have any questions, suggestions, or feedback, please feel free to reach out to me. My GitHub profile is [here](https://github.com/tanvirkhon).
