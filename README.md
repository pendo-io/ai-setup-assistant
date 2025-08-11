### Pendo Installation Assistant 🤖

The Pendo Installation Assistant is a smart tool designed to streamline the integration of Pendo into your application. Simply provide your Pendo snippet, and the assistant will automatically handle the rest, from detecting your application's framework to configuring user data mapping.

---

### How to Use

1.  **Invoke the Assistant:** In a new prompt, type `@pendo-install`.
2.  **Provide Your Snippet:** Paste the Pendo snippet you obtained from your Pendo account.
3.  **Review the Plan:** The assistant will analyze your codebase and propose a complete implementation plan, including snippet placement, initialization logic, and user/account data mapping.
4.  **Confirm and Implement:** Review the proposed changes, confirm they look correct, and the assistant will apply the changes directly to your project.

---

### What It Does Automatically

* **Framework Detection:** Supports popular frameworks like React, Vue, Angular, Next.js, and Nuxt, as well as multi-page applications (MPAs) and micro-frontends.
* **Snippet Placement:** Intelligently places the Pendo loader in the correct file (e.g., `index.html`, `_app.js`, `_document.js`) based on your project's structure.
* **Data Mapping:** Automatically scans your codebase for user and account data, mapping fields like `id`, `email`, and `role` to Pendo's `visitor` and `account` objects. It also detects and includes additional metadata.
* **Configuration Generation:** Creates a complete `window.pendo.initialize()` call tailored to your application's data sources and structure.
* **Implementation & Testing:** Implements the changes and provides a custom checklist to help you validate the installation.

---

### What It Avoids

The assistant is designed to be safe and non-intrusive:

* It **never** exposes sensitive data like passwords or tokens.
* It respects your project's existing code style (e.g., semicolons, quotes).
* It provides a confirmation step before any changes are made to your code.

For more details on the assistant's logic and capabilities, please refer to the detailed prompt document.
