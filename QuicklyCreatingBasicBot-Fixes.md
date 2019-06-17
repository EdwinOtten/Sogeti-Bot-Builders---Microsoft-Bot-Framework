# Microsoft AI School - Tutorial Fix
*For course: Quickly creating a basic bot*

### Before you start
Make sure that you add the *Bot Framework v4 SDK Templates for Visual Studio* extension to Visual Studio.  
1. Within Visual Studio, go to *Manage Extensions* and search online for bot.  
2. *Bot Framework v4 SDK Templates for Visual Studio* should be on top of the list. Install this extension.  

### Step 2 Create a project
1. *Open Visual Studio 2017 from the Start Menu.*  
Visual Studio 2019 is also OK  

### Step 3 Debugging with Bot Framework Emulator
1. *Open the EchoBotBot.cs file.*  
Open Bots/EchoBot.cs  
2. *Put a breakpoint on line 79.*  
Put a breakpoint on line 18.  
6. *Click Open Bot and select the file EchoBot.bot from your source code.*  
Click *Open Bot* and enter "http://localhost:3978/api/messages"  
  
### Step 4 Add Welcome message
1. *Open EchoBotBot.cs and add the following import at the beginning of the file:*  
Open Bots/EchoBot.cs and add the following import at the beginning of the file:  
2. *Modify the OnTurnAsync method, replace the content of the else statement with the following code snippet:*  
Modify the *OnMembersAddedAsync* method, replace the content of the if statement with the following code snippet:
```c#
var msg = "Hi! I'm a restaurant assistant bot. I can add help you with your reservation.";
await turnContext.SendActivityAsync(msg);
```
