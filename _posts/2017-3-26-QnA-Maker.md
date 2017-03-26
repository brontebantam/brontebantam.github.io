---
layout: post
title: Publishing a QnAMaker Bot
published: true
---
As a regular listener to the [.Net Rocks](https://www.dotnetrocks.com) podcast, episode [1410](https://www.dotnetrocks.com/?show=1410) on Chatbots offered a fun mini project idea.

Chatbot offer a new way for users to interact either with a system or business/individual.  The Microsoft Bot framework is one tool to enable developers to build their own bots in Visual Studio.  This is great if you want to create a very bespoke bot using form flow or incoroprating decision logic, but if all you want is a bot to answer questions there is [QnAmaker](https://qnamaker.ai/).

Using the online tool you can quickly have it scan a websites FAQ page or upload your own question and answer file.  Built on top of the Microsoft Bot Framework QnAMaker will then train your data and produce an end point you can use for your Bot which will reply to questions with (hopefully) a suitable answer.

The final piece of the project is to provide an interface.  For this you create a new Bot Service in the Azure Portal and select your QnAMaker template and publish your bot.  The default setup creates a web chat interface for you as embedded below.

But if you want more ways for people to interact then you enable more of the interfaces (Called Channels in Azure), such as Facebook messenger, Slack, Skype etc.  This process is a little bit more invoved, for Facebook for example I had to create a Facebook [Page](https://www.facebook.com/Interviewmebot) and Facebook App, then give my Bot access to the page in Azure by supplying it a Page Authentication token and ID and App ID.

Test out my Bot with the client below, or on [FB Messenger](https://www.facebook.com/Interviewmebot)

<iframe src='https://webchat.botframework.com/embed/interviewmebot?s=juNKaKp35PQ.cwA.Ins.lI9vyDEysoQlQ7O3DPj9TEz9CwWjSCvmBqBDRy1QA6s' height='300px'></iframe>


