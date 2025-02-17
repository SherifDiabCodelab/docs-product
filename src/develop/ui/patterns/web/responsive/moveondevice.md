---
tags: runtime-traditionalweb; 
summary: Move on Device defines where information is displayed thereby improving the display on different devices.
---

# Move on Device

<div class="info" markdown="1">

We’ve been working on this article. Please let us know how useful this new version is by voting.

</div>

You can use the Move on Device UI Pattern to define the placement of information depending on the device.

![](<images/moveondevice-3-ss.png>)

**How to use the Move on Device UI Pattern**

1. In Service Studio, in the Toolbox, search for `Container`.

    The Container widget is displayed.

    ![](<images/moveondevice-6-ss.png>)

    If the UI widget does not display, it may be because you used a ready-made app, which deletes unused widgets from the module. To make additional widgets available in your app:

    a. Go to **Module > Manage dependencies**.

    b. Search for and select the relevant Producer, for example OutSystemsUI. Ensure Show All is selected. 

    c. On the Public elements for the selected Producer displayed on the right, ensure Show All is selected.
    
    d. Search for and select the element you want to add, and click **Apply**. 
    
    e. In Service Studio, in the Toolbox, search for the widget again.

1. From the Toolbox, drag the Container widget into the Main Content area of your application's screen.

    ![](<images/moveondevice-7-ss.png>)

1. On the **Properties** tab, enter the container name.

    ![](<images/moveondevice-9-ss.png>)

1. Repeat steps 2 and 3 for as many containers as you need in your app. 

1. From the Toolbox, drag the Move on Device widget into the Main Content area of your application's screen.

    ![](<images/moveondevice-5-ss.png>)

1. Add the required content to the Move on Device widget.

    In this example, we add an image by dragging the Image widget into the Move on Device widget and selecting an image from the sample OutSystems UI images.

    ![](<images/moveondevice-8-ss.png>)

1. To define where the image appears depending on the device, select the Move on Device widget, and on the **Properties** tab, set the PhoneWidgetId and TabletWidgetId properties.

    ![](<images/moveondevice-2-ss.png>)

After following these steps and publishing the module, you can test the pattern in your app.

## Properties

| Properties |  Description |
|---|---|
| PhoneWidgetId (Text): Optional  | Target container that displays this widget on phones. <p>Examples <ul><li>_Container1.Id_ - The content appears in this container when viewed on a phone</li></ul></p>|
| TabletWidgetId (Text): Optional | Target container that displays this widget on tablets.<p>Examples  <ul><li>_Container2.Id_ - The content appears in this container when viewed on a tablet</li></ul></p>||
