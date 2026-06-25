# Text Utility 🚀

A robust, highly interactive React application built to provide real-time text analysis, manipulation, and extraction tools. Designed with an emphasis on seamless user experience, client-side processing, and dynamic state management.

## 🚀 Tech Stack

*   **Core:** React 18
*   **Build Tool:** Vite
*   **Routing:** React Router v6
*   **Styling & Theming:** Custom CSS with Dynamic Inline Styling (Dark/Light Mode)
*   **Icons:** Bootstrap Icons
*   **HTTP Client:** Axios (Configured for potential API extensions)

## ⭐ Spotlight Feature: Client-Side Data Extraction & Dynamic File Generation

The most technically engaging aspect of this application lies in its ability to process text completely on the client side without relying on backend servers. 

**How it works under the hood:**
*   **Advanced Regular Expressions:** The application implements robust RegExp patterns (`/([a-zA-Z0-9._-]+@[a-zA-Z0-9._-]+\.[a-zA-Z0-9._-]+)/gi`) to instantly scan large blocks of text and extract valid email addresses, demonstrating complex string parsing capabilities.
*   **Dynamic Blob Generation:** Instead of requesting a file from a server, the application leverages the browser's Native `Blob` API. It dynamically converts the user's manipulated text state into a `text/plain` file, generates a temporary `URL.createObjectURL()`, and programmatically triggers a hidden anchor tag to initiate a download. 
*   **Why it's important:** This solves the problem of server load and latency. By keeping file generation and string parsing strictly in the browser, it ensures maximum privacy for the user (their text never leaves their machine) and instant performance.

## 🛠 Features

*   **Real-time Text Metrics:** Instantly calculates word count, character count, and estimated reading time.
*   **Text Manipulation:** One-click transformations for Uppercase, Lowercase, and Sentence Case.
*   **Dynamic Theme Toggling:** A custom-built Dark/Light mode that uses global state to dynamically inject CSS properties and alter the application's aesthetic on the fly.
*   **Clipboard Integration:** Utilizes the `navigator.clipboard` API to allow users to seamlessly copy their formatted text.
*   **Alert System:** A custom, timeout-based notification system to provide immediate, non-intrusive feedback for user actions.

## 💡 Why This Project Stands Out

This project demonstrates a solid mastery of React fundamentals, particularly in managing complex, interdependent state across multiple components. The engineering challenges overcome include handling real-time form inputs efficiently, implementing custom Regular Expressions for data extraction, and interacting with browser APIs (Clipboard and Blob) to create a seamless, app-like experience. It proves competency in creating optimized, serverless architectures where heavy lifting is elegantly handled directly within the client's browser.
