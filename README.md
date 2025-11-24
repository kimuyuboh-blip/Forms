<h1 align="center" style="text-decoration: underline;"><strong>User Registration Form Built With Semantic HTML & CSS</strong></h1>

<p align="center" style="font-style: italic;"> A complete guide to creating and styling semantic, accessible, and well-structured HTML forms. </p>

<h3 style="text-decoration: underline;">Overview</h3>

<p>This project demonstrates how to build a fully semantic registration form and apply professional, scalable CSS styling using:</p>

<ul>
<li>Semantic HTML5 tags (header, main, fieldset, legend, footer)</li>
<li>Accessible form structure with correct labeling</li>
<li>CSS custom properties (variables)</li>
<li>Responsive, consistent form controls</li>
<li>Modern button styling, shadows, and interactive effects</li>
</ul>

<p>The goal is to teach clear structure, accessibility, and clean styling architecture.</p>

<h3 style="text-decoration: underline;">Built With</h3>
<ul>
<li>Semantic HTML5</li>
<li>CSS3 with Custom Properties</li>
<li>No frameworks or external libraries</li>
</ul>


<h3 style="text-decoration: underline;">Getting Started</h3>

<p>This documentation walks you through the structure and styling of the form found in:</p>

<ul>
<li>index.html </li>
<li>styles.css </li>
</ul>

<p>You will learn:</p>

<ul>
<li>How the form is divided into meaningful semantic sections</li>
<li>How inputs, labels, fieldsets, and legends work together</li>
<li>How CSS variables create a scalable color system</li>
<li>How the layout, spacing, borders, and shadows are applied</li>
</ul>


<h3 style="text-decoration: underline;">1. Semantic HTML Structure</h3>

<p>The form uses a clear hierarchical structure:</p>

```

<!doctype html>
<html lang="en">
  <head>…</head>
  <body>
    <header>…</header>
    <main>
      <form>
        <fieldset>Personal Information</fieldset>
        <fieldset>Contact Information</fieldset>
        <fieldset>Preferences & Interests</fieldset>
        <fieldset>Feedback & Additional Information</fieldset>
        <footer>Buttons</footer>
      </form>
    </main>
  </body>
</html>

```

<h3 style="text-decoration: underline;">Why Semantic HTML?</h3>
<ul>
<li>Improves accessibility (screen readers understand the structure)</li>
<li>Improves SEO (logical content hierarchy)</li>
<li>Improves maintainability (sections are clear and manageable)</li>
<li>Supports consistent styling (fieldsets, legends, headers)</li>

</ul>


<h3 style="text-decoration: underline;">2. Section-by-Section Explanation</h3>

<h4>A. Personal Information Fieldset</h4>

Contains fundamental personal details:
<ul>
<li>Text inputs (first name, last name, age)</li>
<li>Date picker (date of birth)</li>
<li>Radio inputs (gender)</li>
<li>File input (profile photo)</li>

</ul>

<h4>Key techniques used:</h4>
<li>Every _"label"_ is linked to its _"input"_ via _"for"_ + _"id"_</li>
<li>Uses appropriate input types (text, date, radio, file)</li>
<li>Autocomplete attributes enhance user experience and accessibility</li>

<h4>B. Contact Information Fieldset</h4>

Uses a mix of:

<ul>
<li>Email + phone inputs</li>
<li>URL input for personal website</li>
<li>Dropdown (select) to choose a country
</li>
<li>Address-related fields (city, street, postal code)</li>
<li>Time input for preferred contact time</li>

</ul>

<h4>Dropdown (select) details:</h4>

```

<select id="country" name="country">
  <option value="kenya">Kenya</option>
</select>

```


Attributes used:

<table>
  <thead>
    <tr>
      <th>Attribute</th>
      <th>Purpose</th>
      <th>Example</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td><code>type</code></td>
      <td>Specifies the input control type</td>
      <td><code>type="email"</code></td>
    </tr>
    <tr>
      <td><code>id</code></td>
      <td>Unique identifier; paired with label</td>
      <td><code>id="first-name"</code></td>
    </tr>
    <tr>
      <td><code>name</code></td>
      <td>Key used when form submits</td>
      <td><code>name="email"</code></td>
    </tr>
    <tr>
      <td><code>placeholder</code></td>
      <td>Inline hint text for the user</td>
      <td><code>placeholder="Enter name"</code></td>
    </tr>
    <tr>
      <td><code>value</code></td>
      <td>Pre-filled default value</td>
      <td><code>value="Kenya"</code></td>
    </tr>
    <tr>
      <td><code>required</code></td>
      <td>Makes the field mandatory</td>
      <td><code>required</code></td>
    </tr>
    <tr>
      <td><code>autocomplete</code></td>
      <td>Browser autofill suggestions</td>
      <td><code>autocomplete="email"</code></td>
    </tr>
    <tr>
      <td><code>disabled</code></td>
      <td>Disables user interaction</td>
      <td><code>disabled</code></td>
    </tr>
    <tr>
      <td><code>readonly</code></td>
      <td>Prevents editing but stays visible</td>
      <td><code>readonly</code></td>
    </tr>
    <tr>
      <td><code>min</code> / <code>max</code></td>
      <td>Range limits (numbers, dates)</td>
      <td><code>min="1" max="10"</code></td>
    </tr>
    <tr>
      <td><code>step</code></td>
      <td>Step increment for sliders/opinions</td>
      <td><code>step="1"</code></td>
    </tr>
    <tr>
      <td><code>accept</code></td>
      <td>Accepted file types in file inputs</td>
      <td><code>accept=".pdf,.doc"</code></td>
    </tr>
  </tbody>
</table>


<h4>C. Preferences & Interests</h4>

Demonstrates more advanced input types:
<ul>
<li>Color picker (type="color")</li>
<li>Range slider (type="range")</li>
<li>Date inputs</li>
<li>Search input</li>
<li>Multiple checkboxes</li>
<li>Education level dropdown</li>
<li>Password + confirm-password fields</li>

</ul>

This fieldset shows how to combine many input types while keeping structure clear and accessible.

<h4>D. Feedback & Additional Information</h4>

Includes:

<ul>
<li>Two textareas</li>
<li>Date-time input</li>
<li>Source of referral dropdown</li>
<li>File upload (resume)</li>
<li>Newsletter and policy checkboxes</li>

</ul>
The section teaches how to work with multi-line text, optional fields, and required agreement boxes.


<h4>E. Footer Button Section</h4>

```
<button name="one" value="register">Register</button>
<button name="two" value="clear">Clear Form</button>

```

The footer wraps the form actions, keeping structure clean and predictable.

<h3 style="text-decoration: underline;">3. CSS Styling System</h3>

All styles originate in styles.css and follow a modular structure using CSS variables.

<h4>CSS Variable System (Color Palette)</h4>

Defined in :root:

<table>
  <thead>
    <tr>
      <th>Variable</th>
      <th>Description</th>
      <th>Hex Value</th>
      <th>Usage</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td><code>--color-bg</code></td>
      <td>Background color</td>
      <td>#f9fafb</td>
      <td>Body background</td>
    </tr>
    <tr>
      <td><code>--color-border</code></td>
      <td>Border color</td>
      <td>#d1d5db</td>
      <td>Inputs, fieldsets, layout borders</td>
    </tr>
    <tr>
      <td><code>--color-text-muted</code></td>
      <td>Muted text</td>
      <td>#6b7280</td>
      <td>Footer text, subtle labels</td>
    </tr>
    <tr>
      <td><code>--color-primary</code></td>
      <td>Main blue</td>
      <td>#2563eb</td>
      <td>Buttons</td>
    </tr>
    <tr>
      <td><code>--color-primary-light</code></td>
      <td>Light blue hover</td>
      <td>#3b82f6</td>
      <td>Register button hover</td>
    </tr>
    <tr>
      <td><code>--color-primary-dark</code></td>
      <td>Deep blue hover</td>
      <td>#1e40af</td>
      <td>Clear button hover</td>
    </tr>
    <tr>
      <td><code>--color-accent-violet</code></td>
      <td>Accent violet</td>
      <td>#8b5cf6</td>
      <td>File input, color picker</td>
    </tr>
    <tr>
      <td><code>--color-accent-pink</code></td>
      <td>Accent pink</td>
      <td>#ec4899</td>
      <td>Shadow highlight</td>
    </tr>
    <tr>
      <td><code>--shadow-primary</code></td>
      <td>Dual-tone shadow</td>
      <td>Violet + Pink</td>
      <td>Form container shadow</td>
    </tr>
  </tbody>
</table>

<h4>Why Variables?</h4>

<ul>
<li>Cleaner, centralized control</li>
<li>Easy theme updates</li>
<li>Consistent color usage</li>
<li>Professional design workflow</li>

</ul>

<h3 style="text-decoration: underline;">4. Form Layout & Element Styling</h3>

Body Container

Uses:

<ul>
<li>Max-width: 600px</li>
<li>Interior padding</li>
<li>Border + soft dual shadow</li>
<li>Background controlled by variables</li>

</ul>

<h4>Input Styling</h4>

All text-like inputs share:

<ul>
<li>Consistent border</li>
<li>40% width</li>
<li>16px font</li>
<li>10px padding</li>
<li>Pointer cursor (interactive feel)
</li>
</ul>

<h4>Select Inputs</h4>

<ul>
<li>Wider (50%)</li>
<li>Larger height (40px)</li>
<li>Clear clickable styling</li>

</ul>

<h4>Textareas</h4>

<ul>
<li>90% width</li>
<li>Consistent padding</li>
<li>110px height</li>
<li>Muted bordered style</li>

<h4>Range Slider</h4>

Fully custom-restyled for:

<ul>
<li>WebKit</li>
<li>Firefox</li>
<li>Edge/IE</li>

</ul>

Includes:

<ul>
<li>Custom track</li>
<li>Custom thumb</li>
<li>Hover enlargement</li>
<li>Clean color usage</li>

</ul>


<h4>File & Color Inputs</h4>

Styled using accent colors:

```
background-color: var(--color-accent-violet);
color: white;
padding: 10px 20px;

```

<h4>Buttons</h4>

```
background-color: var(--color-primary);
transition: background-color 0.5s ease;

```


Hover states:
<ul>
<li>Register → primary-light (blue)</li>
<li>Clear → primary-dark (deep blue)</li>

</ul>


<h3 style="text-decoration: underline;">5. Design Principles Used</h3>
✔ Semantic structure<br>
✔ Consistent spacing and alignment<br>
✔ Variable-driven color architecture<br>
✔ Clean visual hierarchy<br>
✔ Accessible input types<br>
✔ Minimalist modern UI<br>

<h3 style="text-decoration: underline;">Form Preview Screenshot</h3>
<img src="forms.png" alt="Form Preview">

<h3 style="text-decoration: underline;">Usage</h3>

Use this template to build clean, extensible, semantic forms.<br>
Semantic HTML provides:

<ul>
<li>Better accessibility</li>
<li>Cleaner developer workflow</li>
<li>Improved search engine indexing</li>
<li>Easier maintenance and upgrades</li>

</ul>

<h3 style="text-decoration: underline;">Contributing</h3>

Contributions are welcome!<br>
<i style="text-decoration: underline double; font-weight: bold;">Fork → Branch → Commit → PR.</i>

<h3 style="text-decoration: underline;">Contact</h3>

<h3 style="font-weight: bold;">Carlos Kimuyu</h3>

Programming Student | Clean & Modern Web Design

### Contact

- **X (Twitter):** [@KimuyuCarlos](https://twitter.com/KimuyuCarlos)

- **Email:** [kimuyuboh@gmail.com](mailto:kimuyuboh@gmail.com)

- **Project Repository:** [github.com/kimuyuboh-blip/Forms](https://github.com/kimuyuboh-blip/Forms.git)






