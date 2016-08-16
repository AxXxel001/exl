Exl - The expandable list
=========================

Introduction
------------

This module allows you to define Mustache templates that will be used as items in a dynamic list structure. For example this can be used whenever a user should have the ability to edit an unknown number of data fields of the same type.

Example
-------

## Template code
```html
<p>Email Nr. <input id='mail{{exl-full-id}} name='emails[]' type='email' /></p>
```

## HTML Code
```html
<script src='Exl.js'></script>

<h1>Enter your email addresses</h1>
<form>
<exl-container id='emails' template='email-template'></exl-container>
</form>

<script>
	Exl.setupExlContainerWithId('emails');
</script>
```

## Result
![alt text](icon48.png "Logo Title Text 1")