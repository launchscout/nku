# Bueller is Born

due: 1/31/2014

You've been hired to create a classroom management tool called [Bueller](http://www.youtube.com/watch?v=NP0mQeLWCCo).

Here are the stories for the first week of work:

**Creating a student**

```
As a student
I want to add myself to the list of students
So that I can use Bueller
```

1. On the homepage, the student clicks "Create a new student" which takes them
   to the new student page.

2. On the new student page, the student fills in the following text fields:
    * Name
    * Nickname
    * Email
    * Image URL

3. Once the student submits the form, they arrive back at the homepage where
   they see themselves in a list of students and a message telling them that the
   student was successfully created.

**Editing a student**

1. On the homepage, the student clicks on their profile to navigate to the edit
   student page.

2. On the edit student page, the student sees their current information and can
   edit each of their attributes.

3. Once the student submits the form, they arrive back at the homepage where
   they see their updated information and a message telling them that they have
   successfully updated their profile.

```
As a student
I want to edit my profile
So that I keep my information accurate
```

**Viewing the list of students**

```
As a teacher
I want to see a list of students
So I can learn their faces and names
```

4. For each student in the list of students a visitor can see:

   * An image of the student from the Image URL
   * The student's name
   * The student's nickname
   * The student's email

**Gravatr fallback**

Use the following rules to show the student's images on the student index page
(homepage).

1. If a student has an image URL, use that image.

2. If the student has no image URL but has an email address, attempt to get an
   avatar from [Gravatar](http://en.gravatar.com/).

3. If the student has no image URL, and no email address, show a default image
   from Gravatar.

