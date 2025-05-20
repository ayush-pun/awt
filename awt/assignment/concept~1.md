# Web Development Concepts - Part 1

##  HTTP Methods & Status Codes

### HTTP Methods:
- **GET** – Used to retrieve data from the server. Example: Loading a webpage.
- **POST** – Sends new data to the server. Example: Submitting a form.
- **PUT** – Updates existing data entirely.
- **PATCH** – Updates part of the data.
- **DELETE** – Removes data from the server.

### HTTP Status Codes:
- **200 OK** – Request was successful.
- **201 Created** – Data was created successfully (commonly used after POST).
- **400 Bad Request** – Client-side error; request was invalid.
- **401 Unauthorized** – Authentication required or failed.
- **403 Forbidden** – You don't have permission to access the resource.
- **404 Not Found** – The requested resource doesn’t exist.
- **500 Internal Server Error** – Server-side problem occurred.

---

##  CSS Selectors

1. **Element Selector**  
   Targets all elements of a given type.  
   ```css
   p {
     color: blue;
   }
   ```

2. **Class Selector**  
   Targets elements with a specific class.  
   ```css
   .btn {
     background-color: green;
   }
   ```

3. **ID Selector**  
   Targets a single element with a specific ID.  
   ```css
   #header {
     font-size: 24px;
   }
   ```

4. **Descendant Selector**  
   Targets elements inside other elements.  
   ```css
   div p {
     margin: 10px;
   }
   ```

---

##  Git Basics

- **`git init`** – Initializes a new Git repository in the current folder.
- **`git add`** – Adds files to staging (ready to be committed). Example: `git add .`
- **`git commit -m "message"`** – Saves changes to the repository with a message.
- **`git push`** – Sends commits from local to remote repo (e.g., GitHub).
- **`git pull`** – Fetches and merges changes from remote to local.
- **`git clone`** – Copies a remote repo to your machine.
- **`git branch`** – Lists or creates branches.

---

##  Callback & Higher-Order Function

- **Callback**  
  A function passed as an argument to another function to be run later.  
  Example:  
  ```js
  setTimeout(() => {
    console.log("Delayed message");
  }, 1000);
  ```

- **Higher-Order Function**  
  A function that takes another function as a parameter or returns one.  
  Example:  
  ```js
  function greet(callback) {
    callback("Hi!");
  }
  greet(console.log); // Output: Hi!
  ```

---

##  Array Methods

- **`filter()`** – Returns a new array with items that pass a test.  
  ```js
  const nums = [1, 2, 3, 4];
  const evens = nums.filter(n => n % 2 === 0); // [2, 4]
  ```

- **`map()`** – Transforms each element and returns a new array.  
  ```js
  const nums = [1, 2, 3];
  const squares = nums.map(n => n * n); // [1, 4, 9]
  ```

- **`forEach()`** – Executes a function on each array item (no return).  
  ```js
  const names = ["A", "B"];
  names.forEach(n => console.log(n));
  ```

- **`push()`** – Adds items to the end of an array.  
  ```js
  const fruits = ["apple"];
  fruits.push("banana"); // ["apple", "banana"]
  ```

- **`pop()`** – Removes the last item of the array.  
  ```js
  const fruits = ["apple", "banana"];
  fruits.pop(); // ["apple"]
  ```

---

##  Basic HTML Concepts

- **HTML (HyperText Markup Language)** – The structure of web pages.
- **`<h1>` to `<h6>`** – Headings from most to least important.
- **`<p>`** – Paragraph.
- **`<a href="">`** – Anchor tag for links.
- **`<img src="" alt="">`** – Embeds images.
- **`<ul>`, `<ol>`, `<li>`** – Lists (unordered and ordered).

---

##  Basic CSS Concepts

- **Inline CSS** – Styles directly on the element:  
  ```html
  <p style="color: red;">Hello</p>
  ```

- **Internal CSS** – Styles inside `<style>` tags in the HTML head.
- **External CSS** – Linked CSS file using `<link>` tag.
- **Box Model** – Content + Padding + Border + Margin = Box.

---

##  Basic JavaScript Concepts

- **Variables** – `let`, `const`, and `var` are used to store data.
- **Functions** – Blocks of reusable code.  
  ```js
  function greet(name) {
    return `Hello, ${name}`;
  }
  ```

- **Conditionals** – `if`, `else if`, `else` control flow.
- **Loops** – `for`, `while`, and `for...of` to repeat tasks.
- **DOM Manipulation** – Access or modify HTML from JavaScript.  
  ```js
  document.getElementById("myDiv").innerText = "Updated";
  ```

---

##  Mnemonics & Tips

- **HTTP Status 404** – "4-Oh-4? Page no more!" (Page Not Found)
- **Git Order** – "I Add, I Commit, I Push" (init → add → commit → push)
- **CSS ID vs Class** – ID = One (#), Class = Many (.)

---


