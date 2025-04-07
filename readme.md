# Sample Blocks
This plugin was created to demonstrate some block development for WordPress. It's crafted not for use in production, but rather as a distillation of my recent work in this realm. That's right, it's a code sample! I want to demonstrate thought process and spur some questions from you leading to exciting conversations that will result in my employment. Welcome, let's get to it. 

This plugin was developed against the current, as of this writing, version of WP (6.8) and utilizes the `wp-scripts` helpers in the standard way. Only source code has been committed to this repository. You'll want to install dependencies and then run the build script (`npm run build`) before activating the plugin in the WP dashboard.

## Publication Date
This little block of questionable utility stems from a client request made before the post date block existed. (It was introduced into core with version 5.9 and full-site editing.) In the right context, it might still have its uses. Regardless, it makes for a tidy little package to demonstrate an approach to block development.

### Usage
Drop this block into a post via your preferred method and, voila, there's the post date. There are some minor adjustments to be had in the sidebar to control display: the site's default date setting; a handful of other common format choices; arbitrary text to prepend; and a toggle to add/remove the post's modified date. Unlike core's post date block, this block does not allow you to adjust the underlying post date.

### Technical Notes
* Static vs. dynamic. To serialize or not to serialize, that is the question! In an example like this, there's really no right or wrong approach, it depends on the larger context. I chose dynamic since it's a little more involved and makes for nice blend of PHP and JS in single example. Beyond that, I would examine the patterns already in place in an existing codebase and consider goals and use-cases (e.g. client needs, a general release, headless) to guide the decision.

## Document Preview
more to come...