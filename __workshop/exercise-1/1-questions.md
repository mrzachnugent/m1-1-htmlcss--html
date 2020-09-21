# HTML Comprehension Questions

## Q1 - For each of the following HTML documents, is the HTML valid?

Type true/false in the provided [ ].

a) [ True ] `<div><span>hello</div></span>`
<--! It is valid but not semantic -->

b) [ False ]
<--! missing tags -->

```html
<ul>
<li>one</li>
</ol>
```

c) [ True ] `<ul></ul><img/><ol><li>one</li></ol>`
<--! Valid but ul and img are empty -->

## Q2 - What is a screenreader and why should we care about them?

_Feel free to use the powers of Google here, but please provide link(s) to your source(s)_

---

"A screen reader is a form of assistive technology that renders text and image content as speech or braille output. Screen readers are essential to people who are blind, and are useful to people who are visually impaired, illiterate, or have a learning disability".

- [Wikipedia - Screen reader](https://en.wikipedia.org/wiki/Screen_reader)

"[Proper semantics] aids a screen reader user can have is an excellent content structure with headings, paragraphs, lists, etc.

1. The screen reader reads each header out as you progress through the content, notifying you what a heading is, what is a paragraph, etc.
2. It stops after each element, letting you go at whatever pace is comfortable for you.
3. You can jump to the next/previous heading in many screen readers.
4. You can also bring up a list of all headings in many screen readers, allowing you to use them as a handy table of contents to find specific content."

- [MDN web docs](https://developer.mozilla.org/en-US/docs/Learn/Accessibility/HTML)

---

## Q3 - For each of the following cases, which tags will be needed?

a) You want to create a webpage with the photos from your latest vacation

---

`<!DOCTYPE html> <html lang="en" /> <head /> <meta charset="UTF-8" /> <title /> <link rel="stylesheet" href="styles.css"> <body /> <main /> <h1 /> <p /> <img src="./cuba.png">`

b) You want to create a website that lists all the art gallery websites in your city and links to their website.

`<!DOCTYPE html> <html lang="en" /> <head /> <meta charset="UTF-8" /> <title /> <link rel="stylesheet" href="styles.css"> <script src="https://maps.googleapis.com/maps/api/js?key=YOUR_API_KEY&callback=initMap" defer /> <body /> <main /> <h1 /> <p /> <img src="./art.png"> <a href="https://www.artgalleries.com" /> <ul /> <li /> <div id="map" />`

c) You want to sell designer hats. You need to receive orders from the user.

`<!DOCTYPE html> <html lang="en" /> <head /> <meta charset="UTF-8" /> <title /> <link rel="stylesheet" href="styles.css"> <body /> <header /> <nav /> <main /> <h1 /> <h2 /> <p /> <img src="./.png"> <a href="https://www.designerhats.com/checkout" /> <ul /> <li /> <form /> <label /> <input type="text" /> <button /> <input type="radio /> <select /> <optgroup /> <option />`

---

## Q4 - Can a `button` be a child of a `button`? Explain your reasoning

---

No, a `button` cannot be a child of a `button` because it is an inline element. You cannot have an inline element with the same inline element as its parent/ child.

---

## Q5 - What is the most generic tag you can use?

---

The most generic tag that I use is probably a `<div>`. It's just easier to me since I think other container elements have different default css values. I know I have to work on that.

---

## Q6 - What do the following achronyms stand for?

a) `a` --> Anchor

b) `ol` --> Organized list

c) `ul` --> Unordered list

d) `li` --> List item

e) `tr` --> Table row

f) `th` --> Table header

g) `td` --> Table data

## Q7 - Usually, `td` elements are children of what kind of elements?

---

I think that usually, `td` elements are children of `tr`. I haven't really played around with tables.

---

## Q8 - What is the difference between td and th?

---

`th` are at the top (or left) of the columns. They are also bold by default. They are the titles of the rows or columns. `td` are for the data inside that tables. For example, `td` could be numbers inside the table and `th` could explain that those numbers are in millions of dollars.

---

## Q9 - Which tag makes the text appear bigger: h1 or h3?

---

`h1` is bigger by default since it is that main heading. `h3` should be the third header so `h2` is bigger as well and `h4` `h5` `h6` are smaller.

---

## Q10 - In which situation can you use self closing tags?

---

Closing tags are popular in `REACT` (jsx), for [Void-Elements](https://developer.mozilla.org/en-US/docs/Learn/Accessibility/HTML) however, they ending slash is optional in `HTML5`, and in `Q3` where I used them to list elements that I would use in webpages.

---

## Q11 - What is autofilling and why is it important?

---

Autofilling is a function in most code editors like VS Code that allow programmers to type faster and waste less time typing. It shows suggestions to autofill the word that the programmer started typing. It can also be very helpful to help programmers that are having a blank.

---

## Q12 - Which attributes are always present in an img element?

---

- `src` which specifies the path to the image. Without the `src` attribute, there would not be any image present on the webpage.
- `alt` which _should_ always be present. This is important when the image does not load up properly, when the webpage user is using a screan reader and it is important for search engine optimization.

[W3 Schools](https://www.w3schools.com/tags/tag_img.asp)

---

## Q13 - Which attribute is always present for an anchor tag?

---

- `href` which specifies the link/anchor path when the `a` tag element is clicked.
