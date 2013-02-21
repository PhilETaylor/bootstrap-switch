Bootstrap-switch
========================

Demo
----
http://www.larentis.eu/switch/

Usage
-----

Just include Twitter Bootstrap, jQuery, Bootstrap Switch CSS and Javascript
``` html
<link href="http://twitter.github.com/bootstrap/assets/css/bootstrap.css" rel="stylesheet">
<link href="bootstrapSwitch.css" rel="stylesheet">

<script src="https://ajax.googleapis.com/ajax/libs/jquery/1.9.0/jquery.min.js"></script>
<script src="bootstrapSwitch.js"></script>
```

Basic Example
-------------

``` html
<div class="switch">
    <input type="checkbox">
</div>
```

Large, small or mini
--------------------

``` html
<div class="switch switch-large">  <!-- switch-large, switch-small or switch-mini -->
    <input type="checkbox">
</div>
```

Colors
------

``` html
<div class="switch" data-on="danger" data-off="warning">  <!-- primary, info, success, warning and danger -->
    <input type="checkbox">
</div>
```

Animation
---------

``` html
<div class="switch" data-animated="false">
    <input type="checkbox">
</div>
```

Label
-----

``` html
<div class="switch" data-on-label="SI" data-off-label="NO">
    <input type="checkbox">
</div>
```

HTML Label
-----

``` html
<div class="switch" data-on-label="<i class='icon-ok icon-white'></i>" data-off-label="<i class='icon-remove'></i>">
    <input type="checkbox">
</div>
```

Initial values
--------------

``` html
<div class="switch">
    <input type="checkbox" checked="checked" disabled="disabled">
</div>
```

Event handler
-------------

``` javascript
$('#mySwitch').on('switch-change', function (e, data) {
    var $el = $(data.el)
      , value = data.value;
    console.log(e, $el, value);
});
```

Methods
-------

``` javascript
$('#mySwitch').bootstrapSwitch('toggleActivation');
$('#mySwitch').bootstrapSwitch('isActive');
$('#mySwitch').bootstrapSwitch('setActive', false);
$('#mySwitch').bootstrapSwitch('setActive', true);
$('#mySwitch').bootstrapSwitch('toggleState');
$('#mySwitch').bootstrapSwitch('setState', true);
$('#mySwitch').bootstrapSwitch('status');  // returns true or false
$('#mySwitch').bootstrapSwitch('destroy');
```

License
-------
Licensed under the Apache License, Version 2.0
http://www.apache.org/licenses/LICENSE-2.0