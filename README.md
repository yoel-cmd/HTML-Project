# 📝 Conference Registration Form – README

## 📋 Project Overview

This project is a **Conference Registration Form** built with HTML.  
It allows users to register for a conference by filling in personal information, selecting ticket and workshop options, providing payment details, and confirming agreements.

---

## 🎯 Goals

- ✅ Create a clean and accessible HTML form
- ✅ Use semantic HTML elements like `<form>`, `<fieldset>`, and `<legend>`
- ✅ Validate input using built-in HTML attributes
- ✅ Group related fields for clarity and usability
- ✅ Support a dynamic user experience (e.g., conditional fields)

---

## 🏗️ Structure

The form is divided into **4 main sections** using `<fieldset>` and `<legend>`:

1. **Personal Information**
2. **Ticket & Workshops**
3. **Payment Details**
4. **Agreements** *(to be added)*

Each input field is accompanied by a corresponding `<label>` using the `for` and `id` attributes for accessibility and clarity.

---

## ✍️ Form Sections

### 1. 👤 Personal Information

| Field      | Type     | Validation                  |
|------------|----------|-----------------------------|
| Full Name  | `text`   | `required`, `minlength=2`   |
| Password   | `password` | `required`, `minlength=2` |
| Email      | `email`  | `type=email`                |
| Phone      | `tel`    | Custom `pattern` optional   |

---

### 2. 🎟️ Ticket & Workshops

- **Ticket Type**: Dropdown (`select`) with required options:
  - Standard, VIP, Student

- **Workshops**: Multiple checkboxes
  - Web Performance, Accessibility, Testing

- **Diet Preferences**: Radio buttons:
  - None, Vegan, Kosher, Halal, Other  
    - If **Other** is selected → text input appears (`<details>`)

---

### 3. 💳 Payment Details

| Field          | Type       | Validation                                |
|----------------|------------|--------------------------------------------|
| Card Number    | `text`     | `pattern` (13–19 digits, optional spaces) |
| Expiry Date    | `month`    | Must be current month or later            |
| CVV            | `number`   | 3–4 digits (you can use `type=password`)  |

---

## ✅ Validation

- Uses **HTML built-in validation**:
  - `required`
  - `pattern`
  - `minlength`
  - `type=email`, `type=tel`, `type=month`
- Placeholder text for usability
- Tooltips via `title` attribute

---

## ♿ Accessibility & UX

- All inputs are labeled using `<label for="...">`
- Inputs use `autocomplete` where relevant
- Logical grouping via `<fieldset>` and `<legend>`
- Clear placeholders to guide user input

---

## 🧠 Notes

- Form `action=""` is currently empty → you can connect it to a server later.
- This project is **pure HTML** for now. No JavaScript or backend involved.

---

## 📁 File Structure


│
├── index.html ← main HTML form
├── README.md ← you are here

---

## 👨‍💻 Author

Created by [yoelider]  



