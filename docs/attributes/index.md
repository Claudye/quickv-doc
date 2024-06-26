---
sidebar_position: 19
title: Attributes
---
 
# Attributes

Trivule utilizes HTML attributes to configure and customize form validation. These attributes, all of which start with `data-tr`, offer a simple and intuitive approach to define validation rules, events, error messages, CSS classes, and other features related to form field validation. By using these attributes, you can quickly implement form validation in your web applications without needing to write complex JavaScript code. In this documentation, we will explore the most commonly used Trivule attributes, explaining their purpose and providing examples to illustrate their usage.

Trivule Attributes:

1. `data-tr-rules`:
   - Purpose: This attribute allows you to define validation rules for a form field.
   - Use Case: When you need to specify specific conditions for validating a form field, such as minimum or maximum length, date format, regular expression matching, etc.
   - Example: `<input type="text" data-tr-rules="required|email">`

2. `data-tr-events`:
   - Purpose: This attribute allows you to specify trigger events for form field validation.
   - Use Case: When you want to validate a form field when a specific event occurs, such as losing focus, typing text, etc.
   - Example: `<input type="text" data-tr-events="blur|input">`

3. `data-tr-messages`:
   - Purpose: This attribute allows you to define custom error messages for a form field.
   - Use Case: When you want to display specific error messages for each validation rule applied to a form field.
   - Example: `<input type="text" data-tr-rules="required" data-tr-messages="This field is required.">`

4. `data-tr-invalid-class` and `data-tr-valid-class`:
   - Purpose: These attributes allow you to define CSS classes to apply to a form field based on its validation state.
   - Use Case: When you want to apply different visual styles to a form field based on its validity.
   - Example: `<input type="text" data-tr-invalid-class="invalid" data-tr-valid-class="valid">`

5. `data-tr-auto`:
   - Purpose: This attribute allows you to enable or disable automatic validation during input in a form field.
   - Use Case: When you want to validate a form field as the user types data without manually triggering validation.
   - Example: `<input type="text" data-tr-auto="true">`

6. `data-tr-feedback`:
   - Purpose: This attribute allows you to specify a feedback element associated with a form field.
   - Use Case: When you want to display a custom feedback element for a form field, such as an icon or message.
   - Example: `<span data-tr-feedback class="feedback-icon"></span>`

7. `data-tr-submit`, `data-tr-enabled-class`, and `data-tr-disabled-class`:
   - Purpose: These attributes are used to configure the form submission button in relation to validation.
   - Use Case: When you want to enable or disable the submit button based on the form's validity and apply corresponding CSS styles.
   - Example: `<button type="submit" data-tr-submit data-tr-enabled-class="enabled" data-tr-disabled-class="disabled">Submit</button>`

8. `data-tr-name`: 
   - Purpose: This attribute allows you to change the field's name in the error message.
   - Use Case: When you want to use a different name for a field in error messages.
   - Example: `<input type="text" data-tr-name="our conditions">`

9. `data-tr-lang`:
   - Purpose: This attribute allows you to specify the language used for error messages and Trivule's user interface elements.
   - Use Case: When you want to customize the language of error messages and Trivule's user interface.
   - Example: `<form data-tr-lang="fr">...</form>`

Note: Remember to include the Trivule library in your application before using these attributes. You can find the library and code examples on the [Trivule GitHub repository](https://github.com/trivule/trivule).

For more detailed information on using the attributes and other Trivule library features, please refer to the official Trivule documentation.