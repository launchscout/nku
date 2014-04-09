# Project 2 Assignment

Just as we did with the Bueller application, continue to implement features for
your application. As you work, keep your original idea for the minimum feature
set in mind, but don't be afraid to deviate from the plan if needed.

Continuing from last time, write user stories to document the new features of
your application. You might even want to write them first to help keep focused.
Whatever you do, avoid partially implementing many features, leaving your
application in an unworking state. The goal is to always have an application
that a user could actually get value from at all times.

So if I were building a Twitter clone last week I may have the following in my
readme:

------------

**For 4-04 assignment**

```
As a user
I want to write a short blurb and publish it on the web
So that I feel like people are listening to me
```

-----------

For this next assignment I might end up with the following:

-----------

**For 4-04 assignment**

```
As a user
I want to write a short blurb and publish it on the web
So that I feel like people are listening to me
```

**For 4-18 assignment**

```
As as user
I want to follow other users
So that I can see a timeline of all their tweets
```

Testing steps:

1. Sign up two different users.
1. As the first user, navigate to the other user's profile.
1. Click the "follow" button.
1. As the second user, publish a tweet.
1. Sign in as the first user.
1. You should see the other user's tweet on the first user's homepage.

```
As a user
I want to see a list of all the users following me
So that I can see who is listening to me
```

Testing steps:

1. Sign up two different users.
1. As the first user, navigate to the other user's profile.
1. Click the "follow" button.
1. As the second user, click the "followers" link.
1. You should see the other user's avatar and a link to their profile.

```
As a user
I want to favorite a tweet
So that can keep a list of tweets that I enjoy
```

Testing steps:

1. Sign up two different users.
1. As the first user, publish a tweet.
1. As the second user, navigate to the tweet and click "favorite".
1. Click the "favorite tweets" link.
1. You should see your favorited tweet.

```
As a user
I want to see when other people favorite my tweets
So that I can know that other people like what I am writing
```

Testing steps:

1. Sign up two different users.
1. As the first user, publish a tweet.
1. As the second user, navigate to the tweet and click "favorite".
1. As the first user, click "notifications"
1. You should see that the second user favorited the tweet.

-------------------------

How many features to implement is up to you, but Kevin and I will need to make a
subjective call about how substantial your feature set and application are.
Don't try to game the system and create a lot of small features that don't do
much.  We'll be thinking about how the functionality helps users do a "job" and
how valuable it is to them.
