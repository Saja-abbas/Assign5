# 📝 Form Validation with Button Submit (HTML, CSS, jQuery)

A simple yet effective project showcasing how to perform **form validation** when using a button of type `button`, powered by **jQuery** instead of vanilla JavaScript.
In this setup, the form doesn’t auto-submit — instead, **jQuery** manually handles submission after validating all required fields.

---

### 💡 Overview

This project focuses on validating form fields before submission, offering clear user feedback through color-coded messages.
It’s a great example of how jQuery simplifies DOM interactions and event handling for web forms.

---

## 🎯 Core Features

### 🧾 Form Details

The HTML form includes **four mandatory fields**:

* Name
* Phone Number
* Email
* Location

### 🧩 Validation Logic

Implemented using **jQuery**, with two outcomes:

* If any field is empty → a **red warning message** appears below the form.
* If all fields are filled → a **green success message** is shown, and the form is submitted automatically using `form.submit()`.

### 🎨 Styling

The CSS ensures:

* A **centered layout**
* Clean borders and shadows
* A **professional, user-friendly design**

---

## ⚙️ How It Works

1. The form’s submit button has `type="button"` — meaning it won’t automatically submit.
2. When you click **Submit**, jQuery listens for the event via:

   ```js
   $("#subbtn").click(function() { ... });
   ```
3. Inside the click handler:

   * jQuery fetches all input values using `$("#Name").val().trim()` and similar methods.
   * If **any field is empty**, a red warning appears.
   * If **all fields are valid**, a green success message appears, and the following actions occur:

     * The form is reset with `$("#formbody")[0].reset()`.
     * After a short delay, jQuery triggers form submission using:

       ```js
       $("#formbody").submit();
       ```

---

## 🧰 Tech Stack

| Technology | Purpose                                  |
| ---------- | ---------------------------------------- |
| **HTML5**  | Form structure                           |
| **CSS3**   | Layout and styling                       |
| **jQuery** | Event handling and form validation logic |

---

## ✨ Key Takeaway

This project highlights how **jQuery simplifies DOM manipulation**, reduces boilerplate code, and makes **form validation** cleaner and easier to manage — all while keeping the UI responsive and interactive.


