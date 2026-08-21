# LOGIC GATES SIMULATOR
#### Video Demo:  <URL HERE>
#### Description:

**Logic Gates Simulator** is an interactive, lightweight web application designed to demonstrate and simulate the fundamental principles of digital logic and boolean algebra. It allows users to test fundamental logic gates by selecting inputs and observing the calculated logical outputs in real time.

---

### Project Overview & Motivation
In digital electronics and computer science, logic gates are the fundamental building blocks of digital integrated circuits and computer processors. Understanding how basic gates (**AND, OR, XOR, NAND, NOR**) compute binary truth values is an essential foundational concept. 

This project provides a clean, responsive visual interface that computes outputs instantly using client-side JavaScript, eliminating the need for external libraries or server-side dependencies.

---

### Key Features
* **Multi-Gate Support:** Simulates five essential logic gates:
  * **AND Gate:** Outputs `1` only if both inputs are `1`.
  * **OR Gate:** Outputs `1` if at least one input is `1`.
  * **XOR Gate:** Outputs `1` if the inputs are strictly different.
  * **NAND Gate:** Inverts the output of the AND gate.
  * **NOR Gate:** Inverts the output of the OR gate.
* **Instant Dynamic Evaluation:** Uses DOM event listeners (`onchange`) to trigger immediate recalculations whenever inputs or gate types change.
* **Responsive Card UI:** Centered layout styled with pure CSS, compatible across mobile and desktop viewports.

---

### File Structure & Technical Breakdown

#### `index.html`
The entire application is self-contained within this single file to ensure maximum portability and ease of execution:

1. **HTML Layout:**
   * Contains dropdown menus (`<select>`) for selecting the target logic gate and assigning binary values (`0` or `1`) to `Input A` and `Input B`.
   * Houses the result container (`#outputVal`) to present output state clearly.

2. **CSS Styling (`<style>`):**
   * Uses CSS Flexbox (`display: flex`, `justify-content: center`, `align-items: center`) to center the application within the full viewport height (`100vh`).
   * Implements a clean modern card layout with subtle shadows, rounded borders (`border-radius`), and dashed accent borders around the output box.

3. **JavaScript Logic (`<script>`):**
   * **`calculateLogic()`**: Reads input states using `document.getElementById()`, parses values via `parseInt()`, and applies logical and ternary operators (`&&`, `||`, `!==`, `!`) according to standard boolean algebra.
   * Modifies the text content (`innerText`) of `#outputVal` dynamically.
   * Invoked automatically on initial page load to calculate and render the default state immediately.

---

### How to Run the Project
1. Clone or download the repository to your local machine.
2. Open `index.html` directly in any modern web browser (Google Chrome, Firefox, Safari, Edge).
3. No build tools, package managers, or local servers are required.
