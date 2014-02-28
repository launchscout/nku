# Previous attendances

due: 2/28/2014

**Seeing past attendances**

```
As a teacher
I want to view attendances from classes in the past
So that I can see who was in class on a given day
```

1. When any user visits the application they see the student index page showing the attendances for today.

2. On the student index page, the user should see an input field to select a date and a button to submit the search.

3. Selecting a date and pushing the button reloads the page, showing attendances for the selected date.

**1pt Bonus:** Implement a JavaScript datepicker for cross-browser support.

**Note:** It is sufficient to use `<input type="date">` for the date field.


```
As a user
On the students index page I want the date field to default to the currently selected day
So I know what day's attendance I'm looking at
```

1. When a user first visits the student index page they see attendance as it is
   on Today's date. The date field shows today's date.

2. After a user selects a date and submits to see new attendance, the date picker
   shows the currently selected date.


**Seeing all attendances for an individual student**

```
As a teacher
I want to view all attendances for a for a specific student
So that I can see what classes a student has attended
```

1. When any user visits the student index page, they see a link to view all attendances which takes them to the attendance index page.

2. On the attendances index page, a user can sees each student's name as a link.

3. Clicking on a student's name, displays the attendances index page with a list of attendances for that student only.

