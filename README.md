# Amazon Sumerian Bootcamp

## Tutorial 1
Change region to Oregon
Create scene from template: "Default Lighting"
Go to "Import Assets" at the top 
Search for "View Room"
Create Entity "HTML3D"
Open in Editor under the HTML 3D tab in the property pane
Paste in embedded code - make sure all options are desleected or it won't play in the viewer

Create entity: box
Add component: State machine
Add behaviour
name "emit toggleLIght" - naming is important
Add action
Enitty Hover Enter
Add Action 
Set Material Color
Duplicate State
Replace Entity Hover Enter with Entity Hover Exit
Change color for Set MAterial Color for the Entity Hover Exit state
Draw from Start Hover to Stop Hover to craete arrow (click on arrow head to delete arrow)
Add action
Emit Message
Enter Channel (case sensitive)

Key light
Add Emit Message action to both start and stop hover
Go to lights object and add state machine
Add Set Light Properties
Add Listen Message and add channel
Duplicate
Set intensity to 0 for duplicate and rename to lights off

Rim light
Add state machine
Drag toggleLights machine from Assets to Drop Behaviour box

https://us-west-2.sumerian.aws/51a5008882514c54a565098f36638e5e.scene


# Comments
State machine highlighting can be better
Adfd action and Remove is too close. Easy to misclick
