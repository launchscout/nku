# Specification Round Up

due: 3/7/2014

In order align everyone's applications we're going to detail specifications that
may already be implemented in your application. However, most of these
specifications were never documented in the assignments. Step through each one of these
and make sure it is met. When we grade this one we'll step through this list and
look for anything that doesn't meet specifications from previous assignments.

1) Name your project folder `nku-rails`.

   Many students have created different folders in their Nitrous.io box, which is
   totally fine. The only problem is that it is sometimes hard to tell which
   folder contains the assignment.  You can create as many folders as you would
   like, but make sure the assignment is in nku-rails. If you are using the
   Nitrous application to sync your files you can place your nku-rails folder in
   your workspace folder. However, you should not have 2 nku-rails folders.

2) When an anonymous user visits the homepage (or other protected pages) they
   are redirected to the sign in form.

   An anonymous user should only be able to sign in or create a new account.
   Furthermore, an anonymous user should not see the header with links directing
   them to parts of the application that they do not have access to.

   Anonymous users should only be able to see the following pages:

   * New student/user page
   * Sign in page

3) When a logged in student visits the homepage they see the current day's
   seating chart.

4) After a user is successfully logged in they see the seating chart.

5) All users can see a list of all students in the application

   Show all students in the application with their properties:

   * Student Image (from a Gravatar or image_url)
   * name
   * nickname
   * email

   This list is separate from the seating chart.

6) Once logged in, a user should always see a header that contains the following
   links in the following order:

   * Seating Chart - Points to a list of students showing students in seats today
   and absent students
   * All Attendances - Points to the attendance index page
   * Student Index - Points to a list of all students without attendance
   information
   * Edit your profile - Points to the edit student page

7) When a user signs up, they should already be logged in.

   Based on an earlier spec, when students signed up, they would then sign in to
   get access to the application. Now we want to make sure that when a student
   initially signs up, they are already logged in.

8) Remove old blog code

   The Bueller leadership team has decided to abandon the blog features of the
   application. Remove references to posts and comments. Some places to check
   are:

   * In the router
   * In controller files
   * In model files
   * In database tables (create a migration to drop tables)
   * Any view files

9) Student's do not pick their attendance date. The attendance date is
   automatically assigned by the server when students create an attendance.

10) As of now there should be no html `textarea` elements in the application.
   User fields should be represented by text fields. Password fields should be
   html inputs of type `password` to mask user input.

11) In the seating chart the user should be able to see all 4 seat quadrants even
    when there are no attendances.

12) You should not be doing any validation in your controllers. All data
    validation should be performed by models.

13) The seating chart shows students nicknames and pictures.

14) You should not be committing any volatile files to your repository. This
    includes user provided files (if you have any), log files, or any kind of
    user input. Most students don't have any issue with this currently.

15) Your server should be configured to be in the eastern time zone.

16) You should have no inappropriate camelCasing in your code.

