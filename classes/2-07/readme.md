# Class 3

## Schedule

* Review of previous assignment
  * Assignment run-through
  * What problems did people run into?
  * What did people find difficult, easy?

* Let's talk about git commits
  * Setting up your git you use nano
    * git config --global core.editor "nano"
  * Imperative tense
  * Seeing longer commit messages
    * Github
    * git log
    * tig
  * .gitignore

* Idiomatic Ruby
  * snake_case vs CamelCase
  * Database name conventions
    * created_at vs created_on

* Rails
  * Advanced validations
  * ActiveRecord queries

  * The Rails console
  * Generators - Time to stop using them

* Design
  * What should I save in the database vs generate?
  * Dependency Injection
  * Pair programming
  * Test driven development

* Assignment 3 Prep
  * Cleaning up your code
  * Review assignment 3 spec
  * Q & A and spec clarification

## TDD Exercise

```
require 'spec_helper'

FactoryGirl.define do
  factory :student do
    sequence(:name) {|n| "Student Name #{n}"}
    sequence(:email) {|n| "test-#{n}@example.com"}
    password "password"
    password_confirmation "password"
  end
end

describe Student do
  let(:now) { Date.today }

  describe ".in_seat" do
    let!(:student_in_seat_1) do
      attendance = create(:attendance, attended_on: now, seat: 1)
      create(:student, attendances: [attendance])
    end

    let!(:student_in_seat_2) do
      attendance = create(:attendance, attended_on: now, seat: 2)
      create(:student, attendances: [attendance])
    end

    let!(:absent_student) do
      attendance = create(:attendance, attended_on: now - 1.day, seat: 1)
      create(:student, attendances: [attendance])
    end

    specify do
      students = Student.in_seat(1, now)
      expect(students).to include(student_in_seat_1)
      expect(students).to_not include(student_in_seat_2)
      expect(students).to_not include(absent_student)
    end
  end

  describe ".absent" do
    let!(:present_student) do
      attendance = create(:attendance, attended_on: now, seat: 1)
      create(:student, attendances: [attendance])
    end

    let!(:absent_student) do
      attendance = create(:attendance, attended_on: now - 1.day, seat: 1)
      create(:student, attendances: [attendance])
    end

    specify do
      students = Student.absent(now)
      expect(students).to include(absent_student)
      expect(students).to_not include(present_student)
    end
  end
end
```
