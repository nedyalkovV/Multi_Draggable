# Multidraggable
JQuery UI, Multidraggable and selectable extention/lib - this library combine draggable and selectable from JQuery UI and allows you to select and drag multiple elements
___
## Install

#### Dependencies
* **JQuery** - https://jquery.com/
* **JQuery UI** - https://jqueryui.com/

Dowload and load **JQuery** and **JQuery UI** from the links above:
```
<link rel="stylesheet" href="dependencies/jquery-ui.css" media="screen" title="no title" charset="utf-8">
<script src="dependencies/jquery-3.1.0.js" charset="utf-8"></script>
<script src="dependencies/jquery-ui.js" charset="utf-8"></script>
```

Then load **multidraggable.js** or **multidraggable.min.js**
```
<script src="multidraggable.min.js" charset="utf-8"></script>
OR
<script src="multidraggable.js" charset="utf-8"></script>
```

## STRUCTURE

####HTML
```
<ul id="multidraggable">
    <li class="">Red</li>
    <li class="">Blue</li>
    <li class="">Orange</li>
</ul>
```

####JS
```
$('#multidraggable').multidraggable();
```
