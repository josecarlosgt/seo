# Tutorial: Implementing On-page SEO

This document describes the steps for structuring information in an HTML document using HTML5 semantic tags. The content is based on the narrative for the [Laguna Brava Ecotourism Website](https://docs.google.com/document/d/1km0BxhWLX4hsJDRVkEDGWBFxr76Hyf_FNUubJtaPo5c/edit?usp=sharing) created following [the web design process](https://docs.google.com/presentation/d/17QH5RDWIGE9UkEPn0g89vhl6Iw7_nao2lsCcfX6HS2o/edit?usp=sharing) discussed in class.

## Skills
- Optimize Web content by applying on-page SEO techniques

Each task below provides links that explain the purpose of each HTML tag. These links point to two popular learning resources on web development:

- [Mozilla MDN web docs](https://developer.mozilla.org/en-US/docs/Web/HTML/Element). This website contains detailed and up-to-date documentation on HTML.
- [W3Schools](https://www.w3schools.com/) This website contains examples and brief explanations of HTML.

## Preview

![Web page Preview](page-preview.jpg)

Download the [base.zip](https://github.com/josecarlosgt/Web-Design-and-Development/raw/refs/heads/tutorial-2-designing-and-structuring-content-HTML5/base.zip) and complete the following tasks.

## Part I: On-page SEO
On-page Search Engine Optimization (SEO) techniques involve crafting a list of keywords that describe the most relevant and significant aspects of your web page. 

## Task 1: Optimizing the content for keywords
For this page, we will use the following two keywords:
- Laguna Brava
- Things to do

Ensure the page's title and main heading contain the target keywords above.

```html
    ...
    <title>Things to Do in Laguna Brava</title>
    ...
    <h1>Things to Do in Laguna Brava</h1>
    ...
```

> The target keywords should also appear on the web page text. You may also visit the page [How Search organizes information](https://www.google.com/search/howsearchworks/crawling-indexing/) to get a basic understanding of how Google's Search service works.

## Task 2: Add the meta description tag
Provide a description using the [meta tag](https://www.w3schools.com/tags/tag_meta.asp). Make sure you also include your keywords in the description.

```html
<meta name="description" content="Your guide for things to do and activities in  Laguna Brava lake in western Guatemala.">
```

## Task 3: Add image descriptions
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
