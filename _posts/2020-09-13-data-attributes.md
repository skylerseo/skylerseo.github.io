---
title: Data Attributes (유용한 Data-)
author: Skyler Seo
date: 2020-09-13 00:03:00 +0900
categories: [dev, html]
tags: [html, data-, data-attributes]
---

```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Data Attributes</title>
    <style>
      div {
        width: 300px;
        height: 300px;
        background-color: red;
        margin-bottom: 50px;
      }

      div[data-display-name='apple'] {
        background-color: yellow;
      }
    </style>
  </head>
  <body>
    <div data-index="1" data-display-name="apple"></div>
    <div data-index="2" data-display-name="banana"></div>
    <span data-index="1" data-display-name="strawberry">Hi there</span>
    <script>
      const fruit = document.querySelector('div[data-display-name="apple"]');
      console.log(fruit.dataset);
      console.log(fruit.dataset.displayName);
      console.log(fruit.dataset.index);
    </script>
  </body>
</html>
```

# Materials

<https://developer.mozilla.org/en-US/docs/Learn/HTML/Howto/Use_data_attributes>
