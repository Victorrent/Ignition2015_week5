#### Deliverables for week 5 Rails MVC
##### Odin Project Routing Guide Questions:
- What is the "Root" route? 
The root route is where the site lands by default.
- What are the seven RESTful routes for a resource?
Index, show, new, create, edit, update, destroy. 
- Which RESTful routes share the same URL but use different verbs?
Index and create share the /directory URL but use get and post, respectively. Show, update, and destroy all have the same /directory/:id URL with the verbs get, post, and delete.
- How do you specify an ID or other variable in a route?
You need to supply them to the helper methods of those routes.
- How can you easily write all seven RESTful routes in Rails?
resources:posts
- What is the Rails helper method that creates the HTML for links?
link_to "Text you want to show", path_or_url(param - not hardcoded)

##### Odin Project Views Guide Questions:
- What is a layout?
A file that contains the basic structure found in a webpage, a shell.
- What's the difference between a "view template" and a "layout"?
View templates are the overall views of a webpage and live in app/views/controller_name/action_name.html.erb, while layouts are code that is identical across multiple pages, such as the HTML and doctype tags. Layouts live in app/views/layouts
- What is a "Preprocessor"? 
A preprocessor is code executed before the final HTML file is shipped over to the browser.
- Why are preprocessors useful?
Preprocessors add dynamic elements to an otherwise static page, and help solve for code before the view is placed in the browser.
- How do you make sure a preprocessor runs on your file? 
You put the preprocessor file extensions in your file.
- What's the outputted filetype of a preprocessed *.html.erb file? What about a *.css.scss file?
HTML preprocessed through Embedded Ruby and CSS preprocessed through the SASS preprocessor
- What is the difference between the <%= and <% tags?
<%= are if you want something displayed on the page, while <% are for solving code, such as logic.
- What is a view partial?
Files beginning with a "_" that can be used to replicate certain patterns, such as forms.
- How do you insert a partial into your view?
you use <%= render "partial_name" %>
- How can you tell that a view file is a partial?
It has a "_" before the rest of its filename.
- How do you pass a local variable to a partial
You pass in a @variable_name , like a regular variable but with an @ beforehand. Make sure to explicitly pass the partial which variables you want it to have access to. 
- What's the magical Rails shortcut for rendering a User? A bunch of Users?
<%= render user %> <%= render @users %>
- What are asset tags and why are they used?
Helper methods that output HTML tags that are provided by Rails. They allow you to properly render the proper HTML tag based on the name and location.

##### Link to Odin Project Basic Routes, Views and Controllers repo: [my odin repo](<https://github.com/Victorrent/Week_5_Rails_MVC>)
##### Link to Hartl's Rails Tutorial Chapter 5 repo: [my hartl's repo](<https://github.com/Victorrent/Chapter_5_project>)
