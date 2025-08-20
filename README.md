### Pendo Installation Assistant 🤖

The Pendo Installation Assistant is a smart tool designed to streamline the integration of Pendo into your application. Simply provide your Pendo snippet, and the assistant will automatically handle the rest, from detecting your application's framework to configuring user data mapping.

---

### How to Use

1.  **Utilize the Prompt:** Copy the provided prompt to your selected AI tool. 
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

---
### How to Review

After reviewing and deploying, you can use Pendo's built-in developer tools to confirm everything is working as expected.

* Run a check: Open your browser's developer console and run `pendo.validateEnvironment()`.
* Verify the output: Look for the following in the console output `pendo.enableDebugging()`:
  * The visitor.id and account.id are present and correctly formatted.
  * All of the metadata fields you intended to map are listed with their correct values.
* Check the UI: Within a few minutes, you should see data from your test environment appear in your Pendo subscription's Raw Events tab under Settings > Subscription Settings > Applications.

---

This AI prompt is provided to help streamline installation of the Pendo snippet. Please be aware you are solely responsible for reviewing, testing, and deciding whether to deploy any resulting code. Be sure to ensure installation complies with your development, security, privacy, and compliance requirements as Pendo will only process data as instructed by you under your Agreement and DPA. This snippet is provided “as is,” without warranties, and Pendo is not liable for modifications to your codebase or their effects. If you use third-party tools to run the prompt, they are independent services governed by their own terms and Pendo does not control or guarantee their performance.
