---
layout: post

title: Creating and Styling a Contact Form with Next.js and Tailwind CSS
date: 2024-03-19
author: koempelkode
tags: [Next.js, Tailwind CSS, React, Web Development]

tagline: "How to design a responsive Contact Form with Next.js and Tailwind CSS"
categories: 
image: /macbook-pro.png
meta: "Contact Form"
---

In this post, we'll walk through the process of creating and styling a contact form using Next.js and Tailwind CSS.

## Introduction:

Contact forms are a vital component of any website, allowing users to reach out and communicate with site owners or administrators. In this tutorial, we'll create a simple yet effective contact form and style it using Next.js and Tailwind CSS.

## Creating the Contact Form Component:

```javascript
import React from 'react';
import '../Contact/ContactForm.css';

export default function ContactForm() {
  return (
    <form className="container max-w-[50%] space-y-10 p-10">
      <h1 className="pb-5 text-3xl pt-5">Contact</h1>
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
      <div className="block phone">
        <label htmlFor="frm-phone">Phone</label>
        <input
          id="frm-phone"
          type="text"
          name="phone"
          autoComplete="tel"
          required
        />
      </div>
      <div className="name block">
        <div>
          <label htmlFor="frm-first">First Name</label>
          <input
            id="frm-first"
            type="text"
            name="first"
            autoComplete="given-name"
            required
          />
        </div>
        <div>
          <label htmlFor="frm-last">Last Name</label>
          <input
            id="frm-last"
            type="text"
            name="last"
            autoComplete="family-name"
            required
          />
        </div>
      </div>
      <div className="message block pb-4">
        <label htmlFor="frm-message">Message</label>
        <textarea className="" id="frm-message" rows-6 name="message"></textarea>
      </div>
      <div className="button block">
        <button type="submit" className='bg-blue-600 hover:bg-blue-700 duration-300 text-white shadow p-2 rounded-r'>Submit</button>
      </div>
    </form>
  );
}
```

This code snippet defines a `ContactForm` component using React. It consists of input fields for email, phone, first name, last name, and a message, wrapped in a form styled with Tailwind CSS classes.


## Styling the Contact Form:

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

This code snippet defines the CSS styles for the contact form, ensuring a visually appealing and user-friendly design.

## Screenshot:

![Contact Form](contact_form_screenshot.png)

## Conclusion:

In this post, we've created and styled a contact form using Next.js and Tailwind CSS. Contact forms are essential for facilitating communication between users and website owners, and by using Next.js for the frontend and Tailwind CSS for styling, we ensure a seamless user experience.

Stay tuned for more tutorials and code snippets on my blog!