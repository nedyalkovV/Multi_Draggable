# Multidraggable
JQuery UI, Multidraggable and selectable extention/lib - this library combine draggable and selectable from JQuery UI and allows you to select and drag multiple elements

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

## Structure

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
$('#multidraggable').multidraggable([options]);
```
options - type:*object* [optional]

##Methods
> onCreate(event, ui)

 triggers on initialize multidraggable

> onSelecting(event, ui)

triggers on selecting any of elements inside container

> onSelected(event, ui)

triggers when element is selected

> onStopSelecting(event, ui)

triggers when selecting stop no matter if element is selected or not

> onStartSelecting(event, ui)

triggers when selecting start

> onUnselected(event, ui)

triggers when element is unselected

> onUnselecting(event, ui)

triggers while unselecting elements

> onStartDrag(event, ui, elements)

triggers when dragging start

> onDrag(event, ui, elements)

triggers while dragging elements

> onStopDrag(event, ui, elements)

triggers when dragging ends

```
event - starndart jquery event
ui - standart jquery ui
elements - array of html elements
```

#### Example
```
$('#multidraggable-advance').multidraggable({
  containment:'#multidraggable',
  onCreate:(event, ui)=>{},
  onSelecting:(event, ui)=>{},
  onSelected:(event, ui)=>{},
  onStopSelecting:(event, ui)=>{},
  onStartSelecting:(event, ui)=>{},
  onUnselected:(event, ui)=>{},
  onUnselecting:(event, ui)=>{},
  onStartDrag:(event, ui, elements)=>{},
  onDrag:(event, ui, elements)=>{},
  onStopDrag:(event, ui, elements)=>{}
});
```
##Options

Other options except methods remains the same as JQuery UI Documentation such as:

>containment:'div'

>grid:[20,20]

>etc...

##Destroy

>$('#multidraggable').multidraggable('destroy');

##Demo
Demo examples are located in demo directory

##License

Multidraggable is released under the **MIT License**. Have at it.
