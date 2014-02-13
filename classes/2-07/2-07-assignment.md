# Bueller? ... Bueller?

due: 2/14/2014

Now that we have students in our app and we know their identity, we can start
building some more useful features for Bueller. First on the list: attendance.


**Attending class**

```
As a student
I want to log my attendance for a class
So that my teacher knows I'm there
```

1. On the homepage, the student clicks "I'm here!" which takes them
   to the new attendance page.

2. On the new attendance page, the student chooses one of 4 quadrants of the
   room that they are sitting in by entering an integer for their seat number.
   For now we will refer to these quadrants as seats, anticipating that we may
   be able to assign more specific seats going forward.

3. Once the student submits the form, they arrive at an attendance index
   page where they see a message telling them that they have logged their
   attendance.  For each logged attendance in the app, students see:

   * The student's name
   * The date that the attendance was logged
   * The seat number that the student was sitting in

   **Note:** Although you could use the created_at timestamp to show when
   students logged their attendance this is not recommended as it will increase
   the overall difficulty of the assignment, make testing more difficult, and
   make the code more harder to modify in the future. You should create your own
   field (attended_on) to log the attendance date.

   **Note:** Students do not enter their names to log their attendance. You
   should use the currently logged in student when creating attendance.


**Bonus**

Using the [spec in the readme](./readme.md), create a query that will show all
students in a given seat on a given data and a query that will show all absent
students on a given day. In short, if you get the spec passing without
substantially changing it, you've probably accomplished this. Success will earn
you one bonus point.

The bonus will be due by class time on 2/14 so that we can provide the solution
in class.
