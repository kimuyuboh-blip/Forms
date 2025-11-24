<h3 align="center"><strong>User Registration Form Built With Semantic HTML & CSS</strong></h3> 
<p align="center"> A complete guide to creating and styling semantic, accessible, and well-structured HTML forms. </p>

Overview

This project demonstrates how to build a fully semantic registration form and apply professional, scalable CSS styling using:

Semantic HTML5 tags (header, main, fieldset, legend, footer)

Accessible form structure with correct labeling

CSS custom properties (variables)

Responsive, consistent form controls

Modern button styling, shadows, and interactive effects

The goal is to teach clear structure, accessibility, and clean styling architecture.

Built With

Semantic HTML5

CSS3 with Custom Properties

No frameworks or external libraries

Getting Started

This documentation walks you through the structure and styling of the form found in:

index.html 

index

styles.css 

styles

You will learn:

How the form is divided into meaningful semantic sections

How inputs, labels, fieldsets, and legends work together

How CSS variables create a scalable color system

How the layout, spacing, borders, and shadows are applied

1. Semantic HTML Structure

The form uses a clear hierarchical structure:

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

Why Semantic HTML?

Improves accessibility (screen readers understand the structure)

Improves SEO (logical content hierarchy)

Improves maintainability (sections are clear and manageable)

Supports consistent styling (fieldsets, legends, headers)

2. Section-by-Section Explanation
A. Personal Information Fieldset

Contains fundamental personal details:

Text inputs (first name, last name, age)

Date picker (date of birth)

Radio inputs (gender)

File input (profile photo)

Key techniques used:

Every <label> is linked to its <input> via for + id

Uses appropriate input types (text, date, radio, file)

Autocomplete attributes enhance user experience and accessibility

B. Contact Information Fieldset

Uses a mix of:

Email + phone inputs

URL input for personal website

Dropdown (select) to choose a country

Address-related fields (city, street, postal code)

Time input for preferred contact time

Dropdown (select) details:

<select id="country" name="country">
  <option value="kenya">Kenya</option>
  …
</select>


Attributes used:

Attribute	Purpose
name	Defines the form submission key
value	Value sent to backend
required	Ensures user selection
autocomplete	Guides browser autofill
C. Preferences & Interests

Demonstrates more advanced input types:

Color picker (type="color")

Range slider (type="range")

Date inputs

Search input

Multiple checkboxes

Education level dropdown

Password + confirm-password fields

This fieldset shows how to combine many input types while keeping structure clear and accessible.

D. Feedback & Additional Information

Includes:

Two textareas

Date-time input

Source of referral dropdown

File upload (resume)

Newsletter and policy checkboxes

The section teaches how to work with multi-line text, optional fields, and required agreement boxes.

E. Footer Button Section
<button name="one" value="register">Register</button>
<button name="two" value="clear">Clear Form</button>


The footer wraps the form actions, keeping structure clean and predictable.

3. CSS Styling System

All styles originate in styles.css and follow a modular structure using CSS variables.

CSS Variable System (Color Palette)

Defined in :root:

Variable	Purpose	Value
--color-bg	Page background	#f9fafb
--color-border	Input/fieldset borders	#d1d5db
--color-text-muted	Subtle text	#6b7280
--color-primary	Main blue	#2563eb
--color-primary-light	Light blue hover	#3b82f6
--color-primary-dark	Deep hover blue	#1e40af
--color-accent-violet	Violet accent	#8b5cf6
--color-accent-pink	Pink accent	#ec4899
--shadow-primary	Dual-color shadow	violet + pink
Why Variables?

Cleaner, centralized control

Easy theme updates

Consistent color usage

Professional design workflow

🖌 4. Form Layout & Element Styling
Body Container

Uses:

Max-width: 600px

Interior padding

Border + soft dual shadow

Background controlled by variables

Input Styling

All text-like inputs share:

Consistent border

40% width

16px font

10px padding

Pointer cursor (interactive feel)

Select Inputs

Wider (50%)

Larger height (40px)

Clear clickable styling

Textareas

90% width

Consistent padding

110px height

Muted bordered style

Range Slider

Fully custom-restyled for:

WebKit

Firefox

Edge/IE

Includes:

Custom track

Custom thumb

Hover enlargement

Clean color usage

File & Color Inputs

Styled using accent colors:

background-color: var(--color-accent-violet);
color: white;
padding: 10px 20px;

Buttons
background-color: var(--color-primary);
transition: background-color 0.5s ease;


Hover states:

Register → primary-light (blue)

Clear → primary-dark (deep blue)

5. Design Principles Used
✔ Semantic structure
✔ Consistent spacing and alignment
✔ Variable-driven color architecture
✔ Clean visual hierarchy
✔ Accessible input types
✔ Minimalist modern UI

Screenshot
<img src="forms.png" alt="Form Preview">

Usage

Use this template to build clean, extensible, semantic forms.
Semantic HTML provides:

Better accessibility

Cleaner developer workflow

Improved search engine indexing

Easier maintenance and upgrades

Contributing

Contributions are welcome!
Fork → Branch → Commit → PR.

Contact

Carlos Kimuyu
Programming Student | Clean & Modern Web Design

X: https://twitter.com/@KimuyuCarlos

Email: kimuyuboh@gmail.com

Project Repo: https://github.com/kimuyuboh-blip/Forms.git
