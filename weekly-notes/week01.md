Week 1 - May 12 - 17, 2026

May 12-
  MSLearn: Integrate you agent with Microsoft 365, Build agent-driven workflows using Microsoft Foundry, & Develop an AI agent with Microsoft Agent Framework

May 13-
  MSLearn: Orchestrate a multi-agent solution using the Microsoft Agent Framework & Discover Azure AI agents with A2A

May 14-
## Prepare for an AI development project
* Signed into https://ai.azure.com and created a Microsoft Foundry Project
* When I went to deploy the model that the lab recommended I was receiving an "insufficient quota" message.  After a brief look, the model I was trying to use did not have quota built in, so i needed to search for a model with some free usage so I had to use o4-mini instead of the recommended gpt-4.1 to have token allotment quota!
	* The *key* is used for key-based authentication to models and tools (though in most production scenarios you should consider using Microsoft Entra ID authentication based on authenticated user and application identities).
	* The *project endpoint* is used to access models directly in Foundry (including OpenAI models) using the OpenAI **Responses** API, and to access Foundry-specific AAPIs (such as the Foundry Agent service).
	* The *OpenAI endpoint* is used to access models using OpenAI APIs, including the **Chat Completions** API and the **Response** API.
* Installed Foundry Extension in VS code and set my project as the default project!
* Cleaned up resources

Updating git push to reflect correct user name and email.

