# Contributing to Overlay Scrollbars

1. [Getting Involved](#getting-involved)
2. [How To Report style issues](#how-to-report-style-issues)
3. [Core Style Guide](#overlay-scrollbars-style-guide)
4. [Getting Started](#getting-started)

## Getting Involved

There are a number of ways to get involved with the development of this Overlay Scrollbars theme for Stylish. Even if you've never contributed to an Open Source project before, we're always looking for help identifying missing styles or other issues.

## How to Report Style Issues

### I Don't Know CSS
If you don't know CSS very well and have found a missing style, please include as much as possible of following information when opening an issue:

* Screenshot of the problem; include the element(s) in the console if at all possible
  * To select an element, target it with your mouse then right-click and choose "Inspect Element"
  * Please include both the HTML view and the element with the problem in the screenshot (see [issue #119](https://github.com/StylishThemes/GitHub-Dark/issues/119) for an example)

### I Rock at CSS & GitHub!
* Follow the style guide below
* Make any needed changes, then send us a pull request
* Please include a URL to the page (if public)

## Overlay Scrollbars Style Guide

* Use the provided `.editorconfig` file with your code editor. Don't know what that is? Then check out http://editorconfig.org/.
* Limit to the [K&R (KNF variation style)](https://en.wikipedia.org/wiki/Indentation_style#Variant:_BSD_KNF), and **2 SPACE INDENTATION** (no tabs, and not more, and not less than 2 spaces).

  * K&R - KNF Variation Example:
    ```css
    element[attr='value'] {
    ··property: value;
    }
    ```

  * **Not Allman**
    ```css
    element[property='value']
    {
    ··property: value;
    }
    ```

  * Strict space between the `selector` and the `{`:
    ```css
    /* good */
    element[attr='value'] { }

    /* bad */
    element[attr='value']{ }
    ```

  * 2 Space indentation
    ```css
    /* good */
    ··property: value;

    /* bad */
    ····property: value;
    ----property: value;
    ·property: value;
    ```

* Try to wrap lines at around 80 characters.
  * If possible, reduce any added selectors. Remember that Stylus requires an `!important` flag to override default styling, so a selector starting from the body isn't always necessary.
  * Don't add any inline comments. If you want to make a comment, add it as a note in the commit.
  * If your css definition already exists within the style, do not add it again! Add your selector to the existing definition.
* Insert any new css selectors in any available slot before the style definition, or on a new line as needed.
* If you want to add a new userstyle variable, please open an issue and discuss it with us first.

## Getting Started

* [Download](https://github.com/StylishThemes/Overlay-Scrollbars/archive/master.zip), [fork](https://github.com/StylishThemes/Overlay-Scrollbars/fork) or clone this repository.
* Make any changes to the `overlay-scrollbars.user.css` file and save.
Thank you for your contribution!
