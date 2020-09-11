## LocalBindings
Example to show how to use local bindings.

### Description
This sample shows how to connect two UI-Elements via local bindings. The page consists of three stacked panes and a dropDown menu where the dropDown options are connected to the shown pane.

### How to Run
This sample can be run on the Emulator or on a device. After starting, the user interface can be seen at the DevicePage in AppStudio or by using a web browser. The stacked pane which should be shown can then be chosen via the dropDown.
AppStudio version >= 3.0.0 is required.

### Implementation
It is important that the values of the options match the values of the stacked panes. In this sample the values are "first pane", "second pane" and "3. pane".
Choosing the data-content of the options and adding elements to the stacked panes do not change the functionality.
The bindings are achieved by the lines
`<local-binding property="value" name="selectedItem" init="first pane"></local-binding>`
and 
`<local-binding event="change" name="selectedItem"></local-binding>"`
This creates a binding called "selectedItem" which sets the "value" property of the stackedView element. The "init" property is used to set the initially shown pane after the page was loaded.

### More Information
See "UI bindings" tutorial for more information.

### Topics
System, User-Interface, Sample, SICK-AppSpace, Bindings, UI-Builder