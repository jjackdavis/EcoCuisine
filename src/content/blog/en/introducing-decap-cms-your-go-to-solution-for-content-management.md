---
title: "Introducing Decap CMS Your Goto Solution for Content Management"
draft: false
author: Jon Doe
tags:
  - decapcms
image:
  src: /images/decapcms.png
  alt: Decap CMS
snippet: Decap CMS, formerly known as Netlify CMS, is an open-source content
  management system offering developers a seamless way to manage content for
  static site generators.
publishDate: 2023-07-01 23:14
category: Tutorials
---

Decap CMS, formerly known as Netlify CMS, is an open-source content management system that offers developers a seamless way to manage content for static site generators.

## What is Decap CMS?

Decap CMS is a Git-based CMS that allows developers and content creators to add, update, and delete content directly from the git repo of the site. This provides the benefits of version controlled content, allowing for easy rollbacks, branching, and other Git operations.

## Key Features of Decap CMS
---
title: "Banana"
draft: false
author: Fruit
tags:
  - bananas
image:
  src: /images/banana.png
  alt: Banana
snippet: Bananas are a delicious and nutritious fruit loved by many.
publishDate: 2023-07-01 23:14
category: "Fruits"
---

Bananas are a delicious and nutritious fruit loved by many. They are commonly eaten fresh or used in various recipes due to their sweet taste and creamy texture.

## What are Bananas?

Bananas are elongated, curved fruits with a soft, edible flesh inside a thick peel. They grow on banana plants, which are native to tropical regions.

## Nutritional Benefits of Bananas

Bananas are packed with essential nutrients, including:
- **Vitamins**: Bananas are rich in vitamin C, vitamin B6, and vitamin A.
- **Minerals**: They contain potassium, magnesium, and manganese.
- **Dietary Fiber**: Bananas are a good source of dietary fiber, promoting digestive health.

## Culinary Uses of Bananas

Bananas can be enjoyed in various ways:
- **Fresh**: They can be eaten as a quick and nutritious snack.
- **Smoothies**: Bananas are commonly used as a base for smoothies to add sweetness and creaminess.
- **Baking**: They can be used in baking recipes for cakes, bread, and muffins.
- **Desserts**: Bananas are often used in desserts like banana pudding, banana bread, and banana splits.

## Health Benefits of Bananas

Bananas offer several health benefits, including:
- **Heart Health**: The potassium content in bananas may help lower blood pressure and reduce the risk of heart disease.
- **Digestive Health**: The dietary fiber in bananas promotes regular bowel movements and may help prevent constipation.
- **Energy Boost**: Bananas are a great source of carbohydrates, making them an excellent choice for a quick energy boost.

## Buying and Storing Bananas

When buying bananas, look for ones with vibrant yellow skins and no signs of bruising. Store bananas at room temperature, and avoid placing them near other fruits, as they release ethylene gas, which can cause ripening.

In conclusion, bananas are not only delicious but also nutritious, versatile, and easy to incorporate into a healthy diet.

### Open Source

Being open-source means that you have access to the source code and can modify and customize it according to your project requirements. This allows for high flexibility in adapting the CMS to your specific needs.

### Git-Based

Decap CMS uses Git workflows for content management. Every edit becomes a commit, every batch of edits becomes a pull request, and every saved draft is just a branch.

### Easy to Use

Decap CMS provides a user-friendly editorial interface for content creators, freeing them from needing to understand Git or code.

## Getting Started with Decap CMS

Getting started with Decap CMS is as easy as adding two files to your project: `admin/index.html` and `admin/config.yml`.

```html
<!-- admin/index.html -->
<!doctype html>
<html>
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Content Manager</title>
</head>
<body>
  <!-- Include the script that builds the page and powers Decap CMS -->
  <script src="https://unpkg.com/decap-cms@^2.0.0/dist/decap-cms.js"></script>
</body>
</html>
```

```yaml
# admin/config.yml
backend:
  name: github
  repo: owner/repo
media_folder: "img/uploads"
public_folder: "/img/uploads"
collections:
  - name: "post"
    label: "Post"
    folder: "_posts"
    create: true
    fields:
      - {label: "Title", name: "title", widget: "string"}
      - {label: "Body", name: "body", widget: "markdown"}
```

In the era of Jamstack, Decap CMS is paving the way for modern, Git-based content management. With its simplicity and flexibility, it's an excellent choice for developers and content creators alike.
