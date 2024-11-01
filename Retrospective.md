# Retrospective

- name: Simon Wilch
- email: simonwilch@u.boisestate.edu

## Experience

This assigment was relatively easy.. except for one part. After I got the form set up with Pug, you would type in and submit a task to add to the list and it would add it to the database. But, it would load... forever. I checked the code and everything, but nothing seemed wrong. I checked the textbook and it looks like it has to send a response. Then I noticed the function had both req and res. But what do you send back to the code? I initially thought an HTML status code like 200, but the entire web page would simply change to "200 OK". I tried sending the URL back, but I couldn't figure out how to get it out of the response body. I got frustrated. It would simply load forever and the web server would crash. But, I eventually found the redirect response (by scrolling through the autocomplete list, haha). I feel like this isn't the best in porduction environments, since URLs can change or it could get messed up with weird DNS configurations. But in my case, it works! I tested this simply by comparing my work to the example used in the video. I decided to make this look like a real notepad with lines and all that. The lines are actually a repeating gradient!

## Known issues or Bugs

1. If the URL changes, the redirect response needs to be updated.
2. If the user adds a large number of tasks (10+), the words will start to move outside of the lines of the "paper". This was some rough CSS styling, and with more time I could probably have made this more robust.

## Sources used

Nothing besides the provided textbook and example video.
