# Placing students

due: 2/21/2014

On a given day, a teacher should be able to see all of the students in the
classroom.

**Seeing attendance by seat**

```
As a teacher
I want to see a view of all the students in the class today
So that I know who is in class
```

1. When any user visits the application they see the student index page.

2. On the student index page a user sees all of the students in class today
   laid out in their given seat like this:

   +-------------+-------------+
   |Student 1    |             |
   |Student 2    |             |
   +-------------+-------------+
   |Student 3    |             |
   +-------------+-------------+

   where student 1 and student 2 are seat 1 today and student 3 is in seat 3
   today.

   In this layout, a user only sees the student's picture and nickname.

3. On the student index page, a user sees all of the students that are absent
   today.


**One attendance per day**

```
As a teacher
I only want students to create one attendance per day
So that I only see one attendance per student on the seating chart
```

1. Given a student that has already recorded attendance for today, the student
   clicks "I'm here!".

2. When the student fills out the form and tries to create their attendance,
   they see a message telling them that they have already created an attendance
   for today. The new attendance is not created.


**Seat number 1-4 is required for attendance**

```
As a teacher
I want attendance to require a seat number
So that I can see where students are sitting
```

1. When a student logs their attendance without filling out their seat number,
   they see an error message telling them they they must submit a seat number.

3. When a student logs attendance with an out of range number (e.g. 12) they see an
   error message telling them that the seat number must be 1 - 4.

4. When the student submits the form with a non-integer value (e.g. 1.222 or
   "Hello") they see an error message telling them that their seat number must be
   a number.

