# Previous attendances

due: 2/28/2014

**Seeing past attendances**

```
As a teacher
I want to view attendances from classes in the past
So that I can see who was in class on a given day
```

1. When any user visits the application they see the student index page and the attendances for today.

2. On the student index page, the user should see an input to select a past date

3. Selecting a date reloads the page showing attendances for the selected date

4. The datepicker should always default to the currently selected date

**Note:** It is suffiecient to use `<input type="date">`


**Seeing all attendances for an individual student**

```
As a teacher
I want to view all attendances for a for a specific student
So that I can see what classes a student has attended
```

1. When any user visits the student index page, they see a link to view all attendances

2. On the attendances index page, a any user can click on a student's name to view attendances for that student only

3. Clicking a link displays the attendances index page with a list of attendances for only that student

