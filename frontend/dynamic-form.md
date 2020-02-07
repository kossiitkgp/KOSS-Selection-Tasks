# Story
For different events, we use different kinds of forms to fetch data. The forms need not be static. By this we mean, on selecting different options in the middle of the form, furthur fields change\

# Materials
- Bootstrap forms (or any other CSS framework will do, if you can write your custom CSS too)
- Google XD 

# What you need to do
Make a decently good looking form, that validates the fields(pops up error on submitting invalid data like not mentioning mail). 
| Field Name    | Field Type    | Validation Rule  |
| ------------- |:-------------:| -----:|
| Name    |    Input type |Should be a string with length of atleast 2 letters. Compulsory Field |
| Email     | Input type      | Should be a valid mail address format. Compulsory Field |
| Designation | Dropdown containing 2 different Options - `Professor`, `Student` |Compulsory Field |
| Gender    |    Radio Button containing 3 options - `Male`, `Female`, `Others` |Should be a string with length of atleast 2 letters. Compulsory Field |
 
 Based on professor or student, different fields should be shown below
 - If a professor, the below fields will be shown

| Field Name    | Field Type    | Validation Rule  |
| ------------- |:-------------:| -----:|
| Employee ID    |   Input  |Should be a string with length of atleast 8 letters. Compulsory Field |
| Department     | Input type      | Should be a string. Optional Field |

- If a student, the below field should be show

| Field Name    | Field Type    | Validation Rule  |
| ------------- |:-------------:| -----:|
| Roll Number    |   Input  |Should be a string with length of atleast 8 letters. Compulsory Field |
| Department     | Input type      | Should be a string. Optional Field |

A submit Button in the end, which on clicking should validate the form and show errors if any or show success message.

# Tech Stack
You can use what ever the frontend web technologies you are aware of, it can be a stack consist of HTML, CSS, Vanilla JS or Jquery or Typescript, or any frontend framework like React JS, Angular, Vue, or Svelte.js anything you are comfortable with.

# Learning from the task
You should be able to create a form with good UI and good UX, learn how to handle errorenous respones(We get a lot). You will also get a basic understanding of DOM. Event you are not able to complete all the parts of the task, we would like to see your approach in working on different aspects like how you handle errors, how do you show it to the user and the rest.