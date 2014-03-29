# Assignment scores

due: 3/28/2014

While you were working on Bueller, teachers were busy grading assignments in
other legacy applications and spreadsheets.  To get Bueller into production so
that we can start benefiting from the work we've done so far, we need a way to
import assignments and grades from other applications. Also, some teachers
prefer to work in spreadsheets when they grade and want to import this data into
Bueller.

**Importing Assignments**

```
As an administrator
I want to import a list of assignments
So that I can quickly add assignments for students
```

1. On the all assignments page, administrators click on "Upload Assignments" and
   are taken to a screen with a file input field that they can use to upload a
   document.

2. Administrators attach the file with the file input and click on the "Import"
   button. The attached file has a format like this:

    ```
    Email,Assignment Name,Total,Score
    test1@example.com,assignment1,15,8
    test2@example.com,assignment2,15,14
    ```

3. After the file is uploaded the administrator sees "2 assignments were created" and
   are taken to a list of all the assignments where they can see the two listed
   assignments.

**Importing is Itempotent and Updates existing assignments**

1. If the administrator uploads the identical CSV file, no new assignments will
   be created.

2. After uploading the administrator will see "0 assignments were created".

3. If the administrator uploads a similar CSV file with only one new assignment,
   then only one record will be created.

    ```
    Email,Assignment Name,Total,Score
    test2@example.com,assignment2,15,14
    test3@example.com,assignment2,15,12
    ```

4. If the administrator uploads a CSV file that has an updated assignment, that
   assignment will change.

    ```
    Email,Assignment Name,Total,Score
    test1@example.com,assignment2,15,15
    ```

Note: for this feature the identity of the assignment depends on the
combination of its name and email address. So these assignments are considered
the same in the import:

    test1@example.com,assignment2,15,14
    test1@example.com,assignment2,15,15

And these are all different:

    test3@example.com,assignment2,15,14
    test3@example.com,assignment3,15,12
    test2@example.com,assignment3,15,4

**Only administrators can upload assignments**

If a non-admin users visits the page to upload assignments, they are redirected
away from this page.
