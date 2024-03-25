---
layout: post

title: Building a Subscribe Form with Next.js and Tailwind CSS
date: 2024-03-25
author: koempelkode
tags: [Next.js, Tailwind CSS, React, Web Development]

tagline: "How to design a responsive Contact Form with Next.js and Tailwind CSS"
categories: 
image: /macbook-pro.png
meta: "Subscribe Form"
---

In this post, we'll explore how to create a subscribe form using Next.js and Tailwind CSS, similar in structure and design to our previous contact form.

## Introduction:

Subscribe forms are essential for websites looking to engage with their audience and keep them updated on new content or offers. In this tutorial, we'll build a simple yet effective subscribe form that complements our contact form in both structure and design.

## Creating the Subscribe Form Component:

```javascript
import React from 'react';
import '../Subscribe/Subscribe.css';

export default function Subscribe() {
  return (
    <form className="container max-w-[50%] space-y-10 p-10">
      <h1 className="pb-5 text-3xl pt-5">Subscribe</h1>
      <div className="email block">
        <label htmlFor="frm-email">Email</label>
        <input
          id="frm-email"
          type="email"
          name="email"
          autoComplete="email"
          required
        />
      </div>
      <div className="button block">
        <button 
          type="submit"
          className='bg-blue-600 hover:bg-blue-700 duration-300 text-white shadow p-2 rounded-r'
        >
          Sign Up
        </button>
      </div>
    </form>
  );
}
```

## Styling the Subscribe Form:

It's worth noting that the structure and design of this subscribe form are similar to our previous contact form. This consistency in design across different forms on your website can provide a seamless user experience.

```css
.block {
  display: flex;
  flex-direction: column;
}

.name {
  display: flex;
  flex-direction: row;
  justify-content: space-between;
}

.container {
  font-size: 1.3rem;
  border-radius: 10px;
  width: 85%;
  background-color: rgba(255, 255, 255, 0.65); /* Adjust the alpha value (0.5) to change the transparency */
  padding: 20px;
}

.container input {
  font-size: 1.2rem;
  margin: 10px 0 10px 0px;
  border-color: rgb(31, 28, 28);
  padding: 10px;
  border-radius: 5px;
  background-color: #e8f0fe;
}

.container textarea {
  margin: 10px 0 10px 0px;
  border-color: rgb(31, 28, 28);
  border-radius: 5px;
  background-color: #e8f0fe;
  font-size: 20px;
}

.container h1 {
  text-align: center;
  font-weight: 600;
}

.name div {
  display: flex;
  flex-direction: column;
}

.block button {
  padding: 10px;
  font-size: 20px;
  width: 30%;
  border: 3px solid black;
  border-radius: 5px;
}

.button {
  display: flex;
  align-items: center;
}
```

This code snippet defines the CSS styles for the subscribe form, ensuring a visually appealing and user-friendly design.

## Screenshot:

![Subscribe Form](subscribe_form_screenshot.png)

## Conclusion:

In this post, we've created a subscribe form using Next.js and Tailwind CSS, similar in structure and design to our contact form. Subscribe forms are crucial for website engagement, and by using Next.js for the frontend and Tailwind CSS for styling, we ensure a consistent and user-friendly experience for our users.

Stay tuned for more tutorials and code snippets on my blog!
