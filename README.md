# Rails Bug 07

## Setup

* `bundle`
* `rake db:create db:migrate db:seed`
* `rails s`

You can run specs with:

* `rspec`

Note: email/password combinations for existing users populated by `rake db:seed` can be found in the db/seeds.rb file.

## Stories

These bugs are getting a little old, ya know?

<img src="http://openclipart.org/image/300px/svg_to_png/178436/1369219032.png" />

**Tasks start out completed**

OK, here's the latest.  When I create a task, it's automatically marked as done.

Now, I like a list of complete tasks as much as the next person, but this is a little much.

```
As a user
When I create a task
I and I leave the "completed" checkbox unchecked
And I save
Then the task is marked as completed, even though I didn't check the box.
```