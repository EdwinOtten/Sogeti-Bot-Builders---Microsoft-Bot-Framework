# Microsoft AI School - Tutorial Fix
*For course: [Adding Knowledge to your Bot with QnA Maker](https://aischool.microsoft.com/en-us/conversational/learning-paths/building-an-intelligent-bot/adding-knowledge-to-your-bot-with-qna-maker)*

### Step 1-4
Follow steps 1-4 like they are described op AI School.

### Step 5 - Add QnAMaker to the bot
Instead of following the steps described on AI School, do the following:

1. Open the EchoBot project in Visual Studio (you created that earlier)
2. Go to EchoBot.cs
3. Add the following property to the EchoBot class:
```c#
private readonly QnAMaker QnAMaker = new QnAMaker(new QnAMakerEndpoint()
{
    KnowledgeBaseId = "YOUR_KB_ID_HERE",
    EndpointKey = "YOUR_KEY_HERE",
    Host = "YOUR_QNAMAKER_HOST_HERE",
});
```
3. Replace the code in the method `OnMessageActivityAsync` with:
```c#
// Check QnA Maker model
var response = await QnAMaker.GetAnswersAsync(turnContext);
if (response != null && response.Length > 0)
{
    await turnContext.SendActivityAsync(response[0].Answer, cancellationToken: cancellationToken);
}
else
{
    await turnContext.SendActivityAsync("Sorry, I didn't understand that.");
}
```

### Step 6 - Test QnA Maker in Bot Emulator
Follow this step like it is described op AI School.
