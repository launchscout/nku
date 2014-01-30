# Bueller needs a password

due: 2/7/2014

Great job letting your students create their profile. But there's a problem, anyone can change anyones profile!

We need authentication to ensure that students can only update their own profile

**Signing up with a password**

```
As a student
I want to sign up with a password
So that only I can edit my profile
```

1. On the homepage, the student clicks "Sign up" which takes them
   to the new student page.

2. On the new student page, the student fills in the following text fields:
    * Name
    * Nickname
    * Email
    * Image URL
    * **Password** - see [rails has_secure_password](https://www.google.com/search?q=rails+has_secure_password)

3. The students password is encrypted in and saved to the database

4. After the student submits the form, they arrive back at the homepage where
   they are signed in and see themselves in a list of students.

5. The student sees a message saying "Currently signed in as USER_NAME"

**Editing my profile**

```
As a student
I don't want others to edit my profile
So that my information is kept safe
```

1. On the homepage, the student clicks on their profile to navigate to the edit
   student page.

2. Only the currently signed in student can edit their profile.

3. On the edit student page, the student sees their current information and can
   edit each of their attributes.

4. Once the student submits the form, they arrive back at the homepage where
   they see their updated information and a flash message telling them that they
   have successfully updated their profile.

**Signing in**

```
As a student
I want to sign in using my password
So that I can update my profile
```

1. On the homepage, the student clicks "Sign in" to navigate to the new session page.

2. The user enters their email and password and clicks the submit button

3. With a valid password, the users password is authenticated and the user is signed in

4. With an invalid password, the user sees a flash message saying that their password was incorrect

**Signing out**

```
As a student
I want to sign out
So that my little sister can't use my computer to update my profile
```

1. On the homepage, the student click on "Sign out"

2. The user is signed out and cannot edit their profile

