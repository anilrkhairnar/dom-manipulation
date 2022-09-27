![Thumbnail](./Thumbnail.png)

## Task 1

### Target the Top description div and change the DEV Community to `Your_Name` and description to your passion

```javascript
const title = document.querySelector(
  ".side-bar .crayons-card .crayons-subtitle-2"
);

const p = document.querySelector(".side-bar .crayons-card .color-base-70");

// assign new values
title.innerHTML = "Anil Khairnar 👨‍💻";
p.innerHTML = "I Write Code";
```

---

## Task 2

### Fetch all the product name and store in an array

```javascript
const products = document.querySelectorAll(
  ".as-imagegrid--7up .row .as-imagegrid-item"
);

const arr = [];

for (i of products) {
  arr.push(i.innerText.split("\n").shift());
}

console.log(arr);
//['iPhone', 'Mac', 'iPad', 'Watch', 'AirPods', 'Music', 'TV']
```

---

## Task 3

### Add another FAQ 'My New FAQ' to the list

```javascript
// select elements
const parentElm = document.querySelector(".accordion-homepage");

const chiledElm = document.createElement("section");

const h3 = document.createElement("h3");

// create text node
const myFaq = document.createTextNode("My New FAQ");

// append child
h3.appendChild(myFaq);
chiledElm.appendChild(h3);
parentElm.appendChild(chiledElm);

// add class
chiledElm.classList.add("parent");
```

---

## Task 4

### Change the contact number

```javascript
const tel = document.querySelector(".one-tel-number");

tel.innerText = "+91 98765 43210";
```

---

## Task 5

### getElementById, createElement, InnerText, append, setAttribute

```javascript
let btn = document.querySelectorAll(".diwali-deals-product-sale-btn");

btn.forEach((item) => (item.innerText = "Check Out"));
```

---

## Task 6

### Target the search box and on hover change thebackground color to red.

```javascript
const searchBox = document.querySelector(".searchinput___19uW0");

searchBox.addEventListener("mouseover", () => {
  searchBox.style.background = "red";
});
searchBox.addEventListener("mouseout", () => {
  searchBox.style.background = "white";
});
```

---

## Task 7

### First add a text to search in the search bar and then hit the submit search button to search the docs using DOM

```javascript
const input = document.getElementById("top-nav-search-input");
const btn = document.querySelector(".search-button");

btn.addEventListener("mouseover", () => {
  input.value = "javascript event";
  btn.click();
});
```
