## FEATURE:

- AI agent system using a popular Node.js AI library (like LangChain.js or OpenAI SDK) that has another AI agent as a tool.
- Research Agent as the primary agent and an Email Draft Agent as the subagent.
- CLI to interact with the agent system.
- Gmail API integration for the email draft agent, Brave Search API for the research agent.

## EXAMPLES:

In the `examples/` folder, there is a README for you to read to understand what the example is all about and also how to structure your own README when you create documentation for the above feature.

- `examples/cli.js` - use this as a template to create the CLI using Commander.js or similar
- `examples/agents/` - read through all of the files here to understand best practices for creating AI agents that support different providers and LLMs, handling agent dependencies, and adding tools to the agent.

Don't copy any of these examples directly, it is for a different project entirely. But use this as inspiration and for best practices.

## DOCUMENTATION:

- LangChain.js documentation: https://js.langchain.com/
- OpenAI Node.js SDK: https://platform.openai.com/docs/libraries/node-js-library
- Gmail API Node.js: https://developers.google.com/gmail/api/quickstart/nodejs
- Brave Search API: https://brave.com/search/api/

## OTHER CONSIDERATIONS:

- Include a `.env.example`, README with instructions for setup including how to configure Gmail API credentials and Brave Search API.
- Include the project structure in the README.
- Node.js environment has already been set up with the necessary dependencies via npm/yarn.
- Use `dotenv` package and `process.env` for environment variables.
- Consider using TypeScript for better type safety and developer experience.
- Use proper error handling with try/catch blocks for async operations.
- Implement proper logging using a library like Winston or similar.