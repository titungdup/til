`name` attribute is used in form controls (such as `<input>` and `<select>`), as that's the identifier used in the POST or GET call that happens on form submission.

`id` attribute is used whenever you need to address a particular HTML element with CSS or JavaScript.

You may have several radio buttons with different `id` attributes, but the same `name`. When submitted, there is just the one value in the response - the radio button you selected.
