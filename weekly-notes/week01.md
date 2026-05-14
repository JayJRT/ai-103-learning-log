Week 1 - May 12 - 17, 2026

May 12-
  MSLearn: Integrate you agent with Microsoft 365, Build agent-driven workflows using Microsoft Foundry, & Develop an AI agent with Microsoft Agent Framework

May 13-
  MSLearn: Orchestrate a multi-agent solution using the Microsoft Agent Framework & Discover Azure AI agents with A2A

May 14-
Updating git push to reflect correct user name and email.

## Prepare for an AI development project
* Signed into https://ai.azure.com and created a Microsoft Foundry Project
* When I went to deploy the model that the lab recommended I was receiving an "insufficient quota" message.  After a brief look, the model I was trying to use did not have quota built in, so i needed to search for a model with some free usage so I had to use o4-mini instead of the recommended gpt-4.1 to have token allotment quota!
	* The *key* is used for key-based authentication to models and tools (though in most production scenarios you should consider using Microsoft Entra ID authentication based on authenticated user and application identities).
	* The *project endpoint* is used to access models directly in Foundry (including OpenAI models) using the OpenAI **Responses** API, and to access Foundry-specific AAPIs (such as the Foundry Agent service).
	* The *OpenAI endpoint* is used to access models using OpenAI APIs, including the **Chat Completions** API and the **Response** API.
* Installed Foundry Extension in VS code and set my project as the default project!
* Cleaned up resources

## Explore and compare models
* The model leaderboard is a good way to compare models against one another statistically and visually.  
* The tradeoff chart is a good way to visualize the difference between to models for comparison.
* A nice model comparison tool is above the tradeoff tool!
* You can run side by side model comparison with identical prompts!
* You can create evaluation runs with data to test your model against different evaluators.!
* With these reports you can see how the model is performing for the given task as well as run an analysis on the evaluation report to see failures clustered by why they failed.
* After completing the evaluation and running the analysis I deleted the resource group which took all the resources with it.  

## Create a generative AI chat app
* ctrl + shift + p in vs code opens the command pallet
* I did not have the Azure cli PowerShell module on my current machine so I had to download that.
* I hit an error trying to run `python chat-app.py` with a SyntaxError: expected 'except' or 'finally' block and had to troubleshoot that before moving on.  
* I implemented the *ChatCompletions* API first and then modified the code to use the newer *Responses* API.
* I then implemented conversation tracking to the chat app.!
* Next up was streaming responses from the chat app
* I then used the asynchronous API with the chat app which can increase responsiveness of applications when using long-running model or agent operations.

