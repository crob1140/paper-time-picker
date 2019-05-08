paper-simple-time-picker
==========
Simple time picker, compatible with *Polymer 1.0*

Provides a responsive time picker with two dropdown boxes and some keyboard functionality. This
component aims to be a clone of the time picker introduced in Android Lollipop.

Originally branched off bendavis78's https://github.com/bendavis78/paper-date-picker but no longer really resembles the material design spec and original styling or functionality.

## Examples:

Default picker:

```html
<paper-simple-time-picker></paper-simple-time-picker>
```

Setting the initial time to 4:20pm (note that hours given as 24-hour):

```html
<paper-simple-time-picker time="4:20pm"></paper-simple-time-picker>
```

If you include this element as part of `paper-dialog`, use the class
`"paper-simple-time-picker-dialog"` on the dialog in order to give it proper styling.

```html
<paper-dialog id="dialog" modal class="paper-simple-time-picker-dialog"
  on-iron-overlay-closed="dismissDialog">
  <paper-simple-time-picker id="timePicker" time="[[time]]"></paper-simple-time-picker>
  <div class="buttons">
    <paper-button dialog-dismiss>Cancel</paper-button>
    <paper-button dialog-confirm>OK</paper-button>
  </div>
</paper-dialog>
```

# Reporting Bugs

When filing a bug report, please provide an example of how to repoduce using
plunker, jsbin, jsfiddle, etc. You can use the following plunker as a starting
point: http://plnkr.co/edit/gVQluG0GrFP3RzCPZPIi
