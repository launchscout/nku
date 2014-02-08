> **Notice**: This assignment is going to be updated on 2/8/2014, so you may want to hold off any work until you see this notice go away.

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
   room that they are sitting in. For now we will refer to these quadrants as
   seats, anticipating that we may be able to assign more specific seats going
   forward.

3. Once the student submits the form, they arrive back at the student index page
   where they see a message telling them that they have logged their attendance.


**Seeing class attendance**

```
As a teacher
I want to see a list of students that are present today
So that I can learn people's names and faces
```

1. On the homepage, the teacher sees:

  * A diagram showing students with nicknames and pictures in 4 different
    quadrants based on where they are sitting

  * A list of students that are absent from class


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


**Seat number 1-4 is required**

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


**Attendance is cleared each day**

```
As a teacher
I want attendance to be cleared each day
So that I can see attendance for the current day
```

1. Given that students logged attendance yesterday but not today, when I visit the student
   index today I should see that all students are absent.

**Warning**: Features are usually written from a user's perspective without
regard for technical details of an application. Although the client may say
we should "clear out attendance" each day, we should not interpret that to mean
that we should destroy any data about student attendance.
