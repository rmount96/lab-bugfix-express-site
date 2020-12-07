
# (broken) express app :(

This express app has 3 pages, viewable in the browser:

- `/` home page with inspirational graphic
- `/hello` page that just shows "Hello!"
- `/hello/<name>` page that will show "Hello, <name>!" (allowing you to put in anything after the "/hello/")

# Bugs

- [X] All pages show "Page not found"
  - moved 'catch all' to the bottom
- [X] `/hello` route causes an error
  - Fixed typo: req.send needed to send a response instead
- [X] `/hello/world` shows text "Hello, {whom}!" instead of "Hello, world!"
  - Added missing '$' for interpolation

# For the more curious

- Return HTML strings for the `/hello` routes.
- On the `/hello` page, create a list (using `<li>`) of `<a>` tags that go to `/hello/name1`, `/hello/name2`, and `/hello/name3`
  - (Substitute in three real names, of course)
