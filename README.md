# Angular-TODO-app
Todo list application written on Angular 4.

<h2>Functionality</h2>
<h3>No todos</h3>
<p>When there are no todos, <code>#main</code> and <code>#footer</code> should be hidden.</p>
<h3>New todo</h3>
<p>New todos are entered in the input at the top of the app. The input element should be focused when the page is loaded, preferably by using the <code>autofocus</code> input attribute. Pressing Enter creates the todo, appends it to the todo list, and clears the input. Make sure to <code>.trim()</code> the input and then check that it's not empty before creating a new todo.</p>
<h3>Mark all as complete</h3>
<p>This checkbox toggles all the todos to the same state as itself. Make sure to clear the checked state after the "Clear completed" button is clicked. The "Mark all as complete" checkbox should also be updated when single todo items are checked/unchecked. Eg. When all the todos are checked it should also get checked.</p>
<h3>Item</h3>
<p>A todo item has three possible interactions:
<ul>
  <li>Clicking the checkbox marks the todo as complete by updating its completed value and toggling the class completed on its parent <code>&lt;li&gt;</code> </li>
  <li>Double-clicking the <code>&lt;label&gt;</code> activates editing mode, by toggling the .editing class on its <code>&lt;li&gt;</code>
  <li>Hovering over the todo shows the remove button (<code>.destroy</code>)</li>
  </ul>
</p>
<h3>Editing</h3>
<p>When editing mode is activated it will hide the other controls and bring forward an input that contains the todo title, which should be focused (<code>.focus()</code>). The edit should be saved on both blur and enter, and the editing class should be removed. Make sure to <code>.trim()</code> the input and then check that it's not empty. If it's empty the todo should instead be destroyed. If escape is pressed during the edit, the edit state should be left and any changes be discarded.</p>
<h3>Counter</h3>
<p>Displays the number of active todos in a pluralized form. Make sure the number is wrapped by a <code>&lt;strong&gt;</code> tag. Also make sure to pluralize the <code>item</code> word correctly: <code>0 items</code>, <code>1 item</code>, <code>2 items</code>. Example: 2 items left</p>
<h3>Clear completed button</h3>
<p>Removes completed todos when clicked. Should be hidden when there are no completed todos.</p>
<h3>Persistence</h3>
<p>Your app should dynamically persist the todos to localStorage. If possible, use the keys <code>id</code>, <code>title</code>, <code>completed</code> for each item. Make sure to use this format for the localStorage name: <code>todos-[your-last-name]</code>. Editing mode should not be persisted.</p>
<h3>Routing</h3>
Routing is required. The following routes should be implemented: <br>
#/ (all - default),<br>
#/active and<br>
#/completed (#!/ is also allowed). <br>
#/share/XXXX (after opening this route you should immediately redirect to root route #!/). 
When the route changes, the todo list should be filtered and the selected class on the filter links should be toggled. When an item is updated while in a filtered state, it should be updated accordingly. E.g. if the filter is Active and the item is checked, it should be hidden. Make sure the active filter is persisted on reload.</p>
<h3>Share</h3>
<p>App should have “share” button. Add it anywhere to a page. When clicking on it a popup should appear with a textarea containing some link (<code>#/share/XXX</code>). You should somehow encode whole app state in url. When opening this url app should redirect you to the root route and restore state from the link. Don’t forget to add possibility to close the popup.</p>
<h3>Links:</h3>
<p><a href="https://github.com/tastejs/todomvc-app-template">Template</a></p>
