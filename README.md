# Tutorial: Implementing On-page SEO 

In this lab, you will apply several techniques to optimize a web page for search engines. By using HTML elements like headings and meta tags, you will learn how to improve content relevance and visibility in search results.

## Skills
- Optimize Web content by applying on-page SEO techniques

The tasks below provide links that explain the purpose of each HTML tag. These links point to two popular learning resources on web development:

- [Mozilla MDN web docs](https://developer.mozilla.org/en-US/docs/Web/HTML/Element). This website contains detailed and up-to-date documentation on HTML.
- [W3Schools](https://www.w3schools.com/) This website contains examples and brief explanations of HTML.

## Audit your web page for SEO

Download the [base.zip](https://github.com/josecarlosgt/seo/raw/refs/heads/main/base.zip) and audit your web page for common SEO issues using the following tools:

Run:
1. **Pre-audit** — [WR3C Markup Validation Service](https://validator.w3.org/)

- Validates your HTML markup.
- Helps catch structural errors that may affect SEO and browser rendering.

2. **On-Page audit** – [Google Lighthouse](https://developer.chrome.com/docs/lighthouse/)

- Audits your page as rendered in the browser.
- Checks SEO, performance, accessibility, and more.
- Run via Chrome DevTools > Lighthouse tab.

3. **Source code audit** – [Screaming Frog SEO Spider](https://www.screamingfrog.co.uk/seo-spider/)

- Crawls the page and checks the raw HTML and metadata.
- Flags issues such as missing titles, alt attributes, and canonical links.

## Task 1: Optimizing the content for keywords
On-page Search Engine Optimization (SEO) techniques involve crafting a list of keywords that describe the most relevant and significant aspects of your web page. 

For this page, we will use the following two keywords:
- Things to do
- Laguna Brava 

*Things to do* " is a generic keyword that reflects common search intent related to activities, often used by travelers.

*Laguna Brava* is a specific, location-based keyword that narrows the topic to a particular destination in Guatemala.

Combined, they form the phrase "Things to do in Laguna Brava", which reflects a broad intent with a precise context. Using this phrase in titles and headings improves SEO by targeting users who are actively seeking activity-based information for a specific location, improving content relevance and search visibility.

Ensure the page's title and main heading contain the target keywords above.

```html
    ...
    <title>Things to Do in Laguna Brava – Kayaking & Local Tours</title>
    ...
    <h1>Things to Do in Laguna Brava</h1>
    ...
```

> The target keywords should also appear in the web page text. 

## Task 2: Add a meta description and specify the page language
Provide a description using the [meta tag](https://www.w3schools.com/tags/tag_meta.asp). Make sure you also include your keywords in the description.

```html
<meta name="description" content="Your guide for things to do and activities in  Laguna Brava lake in western Guatemala.">
```

Specify the language of your HTML document by adding the lang attribute to the <html> tag. This tells browsers and search engines what language your content is in.

```html
<html lang="en">
```

## Task 3: Specify image descriptions and size
Search engines rely on you providing accurate descriptions of images in the alt text. This will also help your images show up in the results of image-based searches.

```html
    ...
    <img src="img/panoramic-laguna-brava-2.jpg" alt="Panoramic view of lake Laguna Brava" title="Laguna Brava">
    ...
    <img src="img/kayak.jpg" alt="Lake challenge kayak" title="Kayak on Laguna Brava">
    ...
    <img src="img/boat.jpg" alt="Sit Back & Relax boat" title="Boat trip in Laguna Brava">
    ...
...
```

To improve loading performance and reduce layout shifts, make sure to specify the width and height attributes in your <img> tags. This helps the browser reserve the right amount of space for each image while the page is loading. If you don’t include these, the page layout might "jump" as images appear, which can be distracting to users and negatively affect your SEO score, especially in the Cumulative Layout Shift (CLS) metric. Cumulative Layout Shift (CLS) is a measure of how much a web page’s content unexpectedly moves around while it's loading, which can make the page feel jumpy or unstable to users.

```html
    ...
    <img src="img/panoramic-laguna-brava-2.jpg" alt="Panoramic view of lake Laguna Brava" title="Laguna Brava" width="1500" height="369">
    ...
    <img src="img/kayak.jpg" alt="Lake challenge kayak" title="Kayak on Laguna Brava" width="450" height="254">
    ...
    <img src="img/boat.jpg" alt="Sit Back & Relax boat" title="Boat trip in Laguna Brava" width="450" height="254">
    ...
...
```

## Task 4: Make links text descriptive

Update your links to use meaningful, descriptive text instead of generic phrases like "Click here."

Avoid:
```html
    <p>The area around Laguna Brava has been inhabited by Mayan communities of the Chuj ethnicity since the 19th century. <a href="https://en.wikipedia.org/wiki/Chuj_people">Click here</a> to learn more.
    ...
    </p>
```

Use:

```html
    <a href="https://en.wikipedia.org/wiki/Chuj_people">Chuj ethnicity</a>
```

Descriptive link text improves accessibility and helps search engines better understand the context of the linked content.

## Task 5: Add the canonical URL

After you publish your web page to GitHub Pages and get the live URL, add that URL to your HTML page as a canonical link.

A canonical link tells search engines which version of a page is the "main" one. This helps avoid problems if there are duplicate versions of the same page (for example, with different URLs or tracking codes). It also helps Google rank the correct version of your page.

Add the following inside the <head> section of your HTML file:

```html
    <head>
        <link rel="canonical" href="https://example.com/page.html">
    <head>
```

Be sure to replace the URL with the actual one for your published page.
