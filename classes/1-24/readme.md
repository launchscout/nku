# Class 2

## Schedule

* Attendance

* Review of previous assignment
    * Assignment run-through
    * What problems did people run into?
    * What did people find difficult, easy?

* Send an email to Kevin with your Nitrous.io username

* Lecture - What goes where in Rails?

* Nitrous.io migration

* Assignment 2 Prep
    * Review assignment 2 spec
    * Q & A and spec clarification
    * Exercise - Making Gravatar URLs
    * Rails Helpers
    * Object-Oriented Programming in Rails

* Debugging tools


## Migrate your Nitrous.io box

1. In the terminal `cd` into your nku-rails repository
2. Commit any changes in your current repository with `git add .` and `git commit "your
   message"`
3. Go to https://github.com/gaslight/nku-rails and click the "Fork" button
4. On your old box, push your code to the fork you made:
    * `git remote rm origin`
    * `git remote add origin git@github.com:<yourusername>/nku-rails.git`
    * `git push -u origin`
5. On your new box (matches your nku username), click "reveal public key".
6. Copy the key and add it to your Github account ([step #3 here](https://help.github.com/articles/generating-ssh-keys#step-3-add-your-ssh-key-to-github))
7. Login to your new Nitrous.io box
8. git clone your forked Github repo
    * `git clone git@github.com:<yourusername>/nku-rails.git`
9. Your all set. Make sure to use only your new box from now on.
