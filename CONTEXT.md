# OpenAB

OpenAB connects conversations on messaging platforms to coding agents. Its native coding agent is called openab-agent.

## Language

**OpenAB broker**:
The part of OpenAB that connects messaging platforms to coding agents and routes conversations between them.
_Avoid_: Agent, when referring to the broker

**openab-agent**:
OpenAB's native coding agent, which uses a language model and tools to perform tasks on a working project.
_Avoid_: OpenAB broker, ACP wrapper

**Agent session**:
A conversation with a coding agent, including the history and working context used for subsequent requests.
_Avoid_: Platform thread, when referring to the agent's conversation

**Platform thread**:
A conversation thread belonging to a messaging platform, which the broker can associate with an agent session.
_Avoid_: Agent session

**Skill**:
A named set of task instructions that an agent can discover and consult when relevant.
_Avoid_: MCP server, tool

**MCP server**:
A source of external capabilities that an agent can discover and invoke through MCP.
_Avoid_: Skill, model provider

**Model provider**:
The service supplying the language model that an agent uses to interpret requests and choose actions.
_Avoid_: Coding agent, MCP server
