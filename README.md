# hello-world-backbonejs
Getting acquainted with Backbone with a good old "Hello World"

Unlike traditional Views that handle HTML markups, Views are like controllers that process data and link it to templates and ultimately render HTML based on events or data changes.

Properties of Views in Backbone:

-el,
-initialize,
-render,
-events

$el is a cached jQuery object(el) that you can call jQuery functions on and append content.
If this.el is not specified it defaults to an empty div.

render: injects the markup into the elements;

Events: jQuery
$('#new-todo').keypress(createTodoOnEnter);

Events: Backbone
events: {'keypress #new-todo': 'createTodoOnEnter'}

We instantiate a new view with any parameter we need. For the purpose of the Todo app we pass it the todo model.