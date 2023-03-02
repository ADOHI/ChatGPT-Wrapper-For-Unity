# ChatGPT Unity Wrapper
A Unity wrapper for ChatGPT's official API. This wrapper serves as an easy-to-use tool for those looking to explore ChatGPT applications in game development.

## Guide
1. Either download the zip and extract it into an existing Unity project, or clone the repo into your project's Assets directory. <br>
  If you are using a version of Unity that does not support Unity's UI Toolkit, you can just delete the whole UI folder as it's not required.

2. Create an empty game object, and add the "ChatGPTConversation" script to it.
![Screenshot 2023-03-01 at 8 41 26 PM](https://user-images.githubusercontent.com/89364458/222325449-47a833a6-9f10-4583-a78d-69aef54b7e3d.png)

3. Add your API key (you can generate your own key on OpenAI's website), and set your parameters.

4. Use the UnityEvent below the parameters to subscribe something to ChatGPT's response (a function/method that takes a string as an argument).

5. Create a UnityStringEvent somewhere else in your project, and add ChatGPTConversation's method "SendToChatGPT" to the newly created event.

Congrats, now whenever your new UnityEvent is invoked, a request will be sent to ChatGPT's API, and whatever is subscribed to ChatGPT's response will be notified as soon as a response is received. Have fun!


Here's a screenshot of a demo I put together with a simple UI. The UI files are included in the repo, however, you'll have to setup the UnityEvents and plugin the UI elements yourself. If anyone is interested I can also upload the whole project file.
![Screenshot 2023-02-05 at 10 47 13 PM](https://user-images.githubusercontent.com/89364458/216893256-efe3d9e2-fb7d-4833-bae5-9dcb0e9d5717.png)


## Credits
This repo gave me the idea to do this in Unity: <br>
https://github.com/acheong08/ChatGPT
