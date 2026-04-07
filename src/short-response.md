# Short Response Questions

Answer the following questions in your own words. Each response should be 2-4 sentences.

## Question 1: Accessibility

What is accessibility and why does it matter? Name at least two ways that labels make our form inputs more accessible?

**Your Answer:**

Accessibility is making your website available to everyone, anyone who visits your site should able to use it. This matters because people who may have disabilities may have issues accessing your site.

Two ways labels make our form inputs more accessible are by clearly describing what each input is for. Labels that are not properly connected are useful for users with good eyesight, but not for visually impaired users using screen readers. To improve our form inputs, each `<input>` should have a unique id, and each `<label>` should have a for attribute that matches the input’s id, allowing screen readers to correctly read the label.

## Question 2: The `name` vs `id` Attribute

`for`, `name` and `id` are attributes we put on form labels and inputs, but they serve different purposes. Explain what each attribute is used for.

**Your Answer:**
When using labels in our HTML, you can use attributes such as `for` `name`, and `id`. Each one of these attributes serve a different purpose,

When using the attribute `for`, we use this on form labels because it allows you to allocate which input its used for. When `for` is used it basically tells the job its being used for which in this case is a text input through `name`. You give the label the identifier and then use the identifier in the `name` attribute of the input..

The `name` attribute is whats gets sent to the server when the form is submitted, it

When using the attribute `id`, it serves the purpose of its own name, in other words when used on a label and given a name, it applies that name to the label essentially making it identifiable by its purpose. For example

```HTML
<label for="first-name">First Name</label>
<input type="text" id="first-name" name="first-name">
```

## Question 3: Input Types

Why do we use specific input types like `type="email"` or `type="number"` instead of just using `type="text"` for everything? What advantages do they provide?

**Your Answer:**
We use specific input types like `type=email` or `type="number"` instead of just using `type="text"` for everything. The reason is to prevent miss input. It keeps the user from making mistakes on our applications form. For whatever reason lets say a user mistakenly inputs their email under the telephone number field, on our end now we have invalid, false data on the user because they didn't input the correct information, for the sake of the client developers we make it so only a specific type of character can be placed in that field. If the expression is `type="number"` the user will only be able to enter numerical counters, ensuring we get a valid response from the user. The advantages that they provide is validation, the browser automatically checks that the data matches the expected format, and if the format doesn't match it blocks submission.

## Question 4: Form Submission

Form data is typically sent to a server (a computer that receives the data and does something with it). Provide an example of a real web application that uses a form and, to the best of your ability, explain what the application does with that form data.

**Your Answer:**

A real web application that uses a form where data is being sent to a server could be almost any social media platform, for example instagram, facebook, and tiktok. All 3 of these applications have an initial form or a pop up form, they may let you access their website but for certain things you press they may ask you to login and prompt you to a login form page. When you fill out their form to create an account this data gets sent to their servers somewhere in wherever they have them at, these server machines store this data for use anytime you make a comment, like a post, post a picture, or update anything in your profile description. The application sends a request to the server in one of the methods `GET`, `DELETE`, `POST`, `PUT`/`PATCH`.
