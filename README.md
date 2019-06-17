# Sogeti Bot Builders: Microsoft Bot Framework
*Vianen, June 18th 2019*

For this Hands-on event we've prepared two tracks. Both are well documented and the organisers of the event can assist when you run into trouble.
- **Developer track**: involves quite some code, but you end up with a fully functioning chatbot
- **Functional IT track**: you will check out LUIS (Microsoft's Language Understanding platform), explore it's possibilities, and create your own LUIS model.

## Functional IT Track
- Go to [eu.luis.ai](https://eu.luis.ai/applications) and login (or create an account)
- Follow the [Quickstart: Use prebuilt Home automation app](https://docs.microsoft.com/en-us/azure/cognitive-services/luis/luis-get-started-create-app) guide to get started

## Developer Track

### Prerequisites
- Visual Studio [2017 or later](https://www.visualstudio.com/downloads)
- Bot Framework SDK v4 [template for C#](https://aka.ms/bot-vsix)
- [Bot Framework Emulator](https://aka.ms/bot-framework-emulator-readme)

### Getting started
1. Follow the [Quickly creating a basic bot](https://aischool.microsoft.com/en-us/conversational/learning-paths/building-an-intelligent-bot/quickly-creating-a-basic-bot) module (30 minutes)
2. Chat with your bot to check if it's working
3. Try adding a welcome message with `suggested actions` to your bot [[example](https://github.com/microsoft/BotBuilder-Samples/blob/master/samples/csharp_dotnetcore/08.suggested-actions/Bots/SuggestedActionsBot.cs)]
4. Make your bot more intelligent by adding following one of these modules:
    * Follow the [Adding the Language Understanding service to your bot](https://aischool.microsoft.com/en-us/conversational/learning-paths/building-an-intelligent-bot/adding-the-language-understanding-service-to-your-bot) module (70 minutes)
    * Follow the [Adding Knowledge to your Bot with QnA Maker](https://aischool.microsoft.com/en-us/conversational/learning-paths/building-an-intelligent-bot/adding-knowledge-to-your-bot-with-qna-maker) module (40 minutes)
