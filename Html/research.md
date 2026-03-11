# Research Answers

## 1. GET vs POST

**GET**

* Sends data in the **URL**.
* Used to **retrieve data**.
* Not good for sensitive information because the data appears in the address bar.

**POST**

* Sends data in the **request body**.
* Used to **send important data to the server**.
* More secure than GET.

**For register.html:**
I would use **POST** because the user will send personal information like name, email, and password, so it is safer than GET.

---

## 2. Semantic HTML

Using tags like `<header>`, `<main>`, `<section>`, and `<footer>` is better than using only `<div>` because:

* It makes the **structure of the page clear**.
* It helps **search engines understand the content**.
* It improves **accessibility**.
* It makes the code **easier to read**.

---

## 3. The Request / Response Cycle

1. The browser asks **DNS** to find the **IP address** of google.com.
2. DNS returns the IP address.
3. The browser sends an **HTTP request** to that IP.
4. The server sends back an **HTTP response** with the webpage files.
5. The browser loads the files and displays the page.
