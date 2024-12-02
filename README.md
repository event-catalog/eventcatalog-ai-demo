# EventCatalog AI Demo

This is a proof of concept demo of how to use AI to ask questions about your EventCatalog.

This demo uses [git2txt](https://github.com/addyosmani/git2txt) to extract the text from the git repo and uses this for the LLM context.

How to run the demo:

1. Clone the repo or [Create your own EventCatalog](https://www.eventcatalog.dev/)
2. Run `npx git2txt https://github.com/event-catalog/eventcatalog-ai-demo` (replace with your repo)
3. Open your AI Agent and add the context from the previous step.
4. Ask questions about your EventCatalog!

Things to note:
If your Catalog is large, you may need to increase the context window of your LLM.

Some prompts to try:

Setup the model:

```
You are an expert at EventCatalog. You are helping a developer understand their event-driven architecture.
Use the markdown files in the repo to answer the question.
```

Example questions:
- "What events do we have in our system"
- "Who owns these events? and how can I contact them?"
- "I have a new feature I want to add, I want to add it when a user signs up, do we have an event for that?"
- "What domains do we have?"
- "Create me Java model for the PaymentProcessed event"
- "What channels do we have?"

## Get these features with EventCatalog

We are working on [EventCatalog Studio](https://studio.eventcatalog.dev/), a visual designer for event-driven architectures.

You can sign up for the beta [here](https://eventcatalog.dev/studio).

License: MIT