Given a form the plugin will find all the fields and store their associated <label> text using jQuery's .data() method.

This means it requires inputs to have an 'id' and an associated label using the 'for' attribute, e.g.

    <form action="#" method="post">
        <label for="example">Example Label</label>
        <input type="text" id="example" />
    </form>
	
It can then be initiated like this:

    $('form').inFieldLabels();
	
The method also accepts a filter parameter in case you want to limit the in-field labels to specific elements or :not(specific elements):

    $('form').inFieldLabels('.in-field-label');
	
More documentation can be found [here](http://richardscarrott.co.uk/posts/view/jquery-in-field-labels "More info on the jQuery in-field-labels plugin")