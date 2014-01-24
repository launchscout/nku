# Class 2

## Schedule

* Attendance

* Review of previous assignment
    * Assignment run-through
    * What problems did people run into?
    * What did people find difficult, easy?

* Nitrous.io migration

* Lecture - What goes where in Rails?

* Assignment 2 Prep
    * Review assignment 2 spec
    * Q & A and spec clarification
    * Exercise - Making Gravatar URLs
    * Rails Helpers
    * Object-Oriented Programming in Rails


## Migrate your Nitrous.io box

1. In the terminal `cd` into your nku-rails repository
2. Commit any changes in your current repository with `git commit -am "your
   message"`
3. Go to https://github.com/gaslight/nku-rails and click the "Fork" button
4. Change your origin remote to the new fork you made:
    * `git remote rm origin`
    * `git remote add origin git@github.com:<yourusername>/nku-rails.git`
5. `git push -u origin`
6. Mitch needs to make sure you've been invited to your new Nitrous.io box
7. Login to new Nitrous.io box
8. git clone your Github repo
    * `git clone git@github.com:<yourusername>/nku-rails.git`
