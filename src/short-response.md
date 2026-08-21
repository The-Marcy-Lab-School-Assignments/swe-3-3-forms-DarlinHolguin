# Short Response Questions

Answer the following questions in your own words. Each response should be 2-4 sentences.

## Question 1: Accessibility

What is accessibility and why does it matter? Name at least two ways that labels make our form inputs more accessible?

**Your Answer:**

Accessibility is making your website available to everyone, anyone who visits your site should be able to use it. This matters because people who have disabilities may have issues accessing your site.

Two ways labels make our form inputs more accessible are by clearly describing what each input is for. Labels that are not properly connected are useful for users with good eyesight, but not for visually impaired users using screen readers. To improve our form inputs, each `<input>` should have a unique id, and each `<label>` should have a for attribute that matches the input's id, allowing screen readers to correctly read the label.

## Question 2: The `name` vs `id` Attribute

`for`, `name` and `id` are attributes we put on form labels and inputs, but they serve different purposes. Explain what each attribute is used for.

**Your Answer:**

When using the attribute `for` we use it on form labels because it allows for us to connect the label to a specified input. The value of `for` has to match the `id` that the input is describing. Screen readers announce the label when the input is focused so clicking the label will then focus on its input.

When using the `id` attribute it is placed on the input and gives it a unique identifier. This is the value that the for attribute matches to, which is what creates the connection between both elements.

When using the `name` attribute its what gets sent to servers when the form is submitted. What it does is that it labels the data so that when the data from the form that was just submitted arrives at the server, each value can be identified by its name.

For example -

```HTML
<label for="first-name">First Name</label>
<input type="text" id="first-name" name="first-name">
```

## Question 3: Input Types

Why do we use specific input types like `type="email"` or `type="number"` instead of just using `type="text"` for everything? What advantages do they provide?

**Your Answer:**
We use specific input types like `type="email"` or `type="number"` instead of just using `type="text"` for everything. The reason is to prevent mis-input. It keeps the user from making mistakes on our applications form. For whatever reason let's say a user mistakenly inputs their email under the telephone number field, on our end now we have invalid, false data on the user because they didn't input the correct information. For the sake of the client developers we make it so only a specific type of character can be placed in that field. If the expression is `type="number"` the user will only be able to enter numerical counters, ensuring we get a valid response from the user. The advantages that they provide are validation, the browser automatically checks that the data matches the expected format, and if the format doesn't match it blocks submission.

## Question 4: Form Submission

Form data is typically sent to a server (a computer that receives the data and does something with it). Provide an example of a real web application that uses a form and, to the best of your ability, explain what the application does with that form data.

**Your Answer:**

A real web application that uses a form where data is being sent to a server could be almost any social media platform, for example instagram, facebook, and tiktok. All 3 of these applications have an initial form or a pop up form, they may let you access their website but for certain things you click they may ask you to log in and prompt you to a login form page. When you fill out their form to create an account this data gets sent to their servers somewhere wherever they have them, these server machines store this data for use anytime you make a comment, like a post, post a picture, or update anything in your profile description. The application sends a request to the server in one of the methods `GET`, `DELETE`, `POST`, `PUT`/`PATCH`.
