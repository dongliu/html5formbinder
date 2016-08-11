# html5formbinder

When a form is submitted via AJAX, we need to serialize the form data, and send it to the server. Often, a user would like to save a partially finished form, and continue to work on the form later. Then the form needs to load the saved data on the server. If the data is retrieved via AJAX, the data needs to bind to the form. This JavaScript library provides a two-direction data binder in JSON format for HTML5 forms.

## Specs

The HTML5 form is defined in [the 4.10 section](http://www.w3.org/TR/html5/forms.html) of the W3C specification. This binder covers three types of HTML5 form elements: `input`, `textarea`, and `select`. The binder converts the data input by a user in an element into a simple type or an array of simple type in JSON.

### textarea

```
textarea <==> string
```

### select

```
select(type='select-one') <==> string
select(type='select-multiple') <==> [string]
```

### input

```
input(type='hidden') <==> string
input(type='text') <==> string
input(type='tel') <==> string
input(type='url') <==> string
input(type='email') <==> string
input(type='password') <==> string
input(type='date') <==> string
input(type='time') <==> string
input(type='number') <==>  string
input(type='range') <==>  string
input(type='color') <==> string
input(type='checkbox') <==> boolean
input(type='radio') <==> string
input(type='radio') <==> string
input(type='radio') <==> string
input(type='submit')  <==> string
input(type='reset')  <==> string
input(type='button')  <==> string 
input(type='image')  ==> undefined
input(type='file')  ==> undefined


```
