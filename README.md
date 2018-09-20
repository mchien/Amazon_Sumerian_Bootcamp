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

# Tutorial 3
CloudFormation - Infrastructure as code
https://console.aws.amazon.com/cloudformation/home?region=us-east-1#/stacks/create/review?templateURL=https:%2F%2Fs3.amazonaws.com%2Fsumerian-cfn-templates%2FLexPollyExampleTemplate.yml&stackName=AmazonSumerianLexPollyTutorialStack
Cognito in aws - manage credentials in identity pool e.g. login flow
Lex - chatbot, natural text processing services
Polly - speech services

Create new Speech & Gestures scene
paste in CognitoIdentityPoolID into AWS COnfiguration tab in world properties
Host > Point of interst- look at default camera
Host > Animate using speech - lipsync and gestures
Speech > Introspeech

# Tutorial 4
Amazon Lex
Custom bot - 5 min, no to agreement
Intents -> add intent -> name is case sensitive
Fill in intent phrases (utterances)
Slot types
create new slot
Slot type name
Restrict to Slot values and Synonyms
enter synnonyms
slot type drop down - list of amazon supported slots
save intent
change prompt for what you want Lex to say
add response with text and {} to replace with slot type
build

New scene/entity
Add component : dialogue
Name is name but dev alias is $LASTEST
send audio, get back lex, sumarian reads text
add component: speech
add component: state machine


# Comments
State machine highlighting can be better
Adfd action and Remove is too close. Easy to misclick
can you interrupt gestures
can you speed up gestures
