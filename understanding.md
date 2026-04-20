Anthropic has 3 types of models: like categories

1> Haiku -- llm model -- smallest model -- designed for tasks that require less context and faster response times.
2> Sonnet -- llm model -- balanced model -- designed for a wide range of tasks that require moderate context and response times.
3> Opus -- llm model -- largest model -- designed for complex tasks that require extensive context and detailed responses.

all of the models starts with claude 

claude desktop -- a user interface for interacting with the models on a desktop environment.
claude code -- a specialized version of the models designed for coding tasks, providing assistance with programming and software development.

claude code is agentic graph which uses claude llms under the hood.


claude code components:
1> Agentic graph -- a framework for building and executing complex workflows using the capabilities of the claude llms.
2> Tools -- specific functionalities or APIs that can be integrated into the agentic graph to enhance its capabilities, such as web browsing, database access, or code execution.

SKILLLS: amazing powers to normal agentic graph, such as the ability to use tools, access external data sources, and perform complex reasoning tasks. These skills enable the agentic graph to handle a wide range of tasks and provide more comprehensive and accurate responses.
handle repetative tasks

always create skills i nside ,claude folder

EXTENDING THE SKILLS:
adding scripts
adding references
adding examples

new feature:
claude code helps us to create the skills as well
skill-creation -- a feature that allows users to create new skills for the agentic graph using the capabilities of the claude code model. This feature provides a user-friendly interface for defining the functionality and behavior of new skills, making it easier to extend the capabilities of the agentic graph.
we have to use pluggins for that 
in claude code terminal search agents --> manage agents --> market place --> vs code teminal run thiose commands --> and then in plugins awitch it ON and then you can create the skills using claude code model.

Sub Agents:
Sub agents are specialized agents that can be created within the agentic graph to handle specific tasks or domains. 
These sub agents can be designed to focus on particular areas of expertise, allowing for more efficient and accurate responses when dealing with complex queries or tasks that require specialized knowledge. 

Agent Team (its in Beta verison):
Agent teams are a collection of sub agents that work together to accomplish a goal or task.

claude code is also used to know the project when you are newly onboparded to the project and you want to know about the project and its structure. 
You can ask claude code about the project and it will give you the details about the project and its structure. 
It will also give you the details about the files and folders in the project and their purpose. 
This feature is very useful for new members of the team to get familiar with the project quickly.

btw commands for claude code terminal:
Use /btw to ask a quick question about your current work without adding to the conversation history. 
This is useful when you want a fast answer but don’t want to clutter the main context or derail Claude from a long-running task.

/btw type your question here

/voice -- a command that allows you to enable voice input and output in the claude code terminal. 
This feature enables you to interact with the agentic graph using voice commands and receive responses in audio format, 
enhancing the user experience and making it more convenient for hands-free interactions.

schedule prompts:
Schedule prompts allow you to set up specific prompts to be executed at predetermined times or intervals. This feature is useful for automating tasks, sending reminders, 
or performing regular checks without manual intervention. You can define the prompt, specify the timing, and Claude will execute the prompt as scheduled, 
providing you with the necessary information or actions at the right time.

using /loop 3m and you can give the cron syntax

we can disaqble these schedulars using env variables also  --> taht needs to explore

plugins and market places:
plugins are the additinal functionality to the claude code
market place is the place where you can find the plugins and install them in your claude code terminal to use them in your agentic graph.

custom plugins (clustom skills) also availabkle

two most popular for skills are 
skillsmp.com
smithery.ai

MCP - MODEL CONTEXT PROTOCOL:
standard we have in the AI industry not soleny for claude code.
it is build by anthropic

btw/ claude code have some built in tools like read write grep.. refer for further information.

🌍 1. Normal (manual) APIs
👉 Purpose: share data/services between systems

🤖 2. MCP (current usage)
👉 Purpose: help AI access YOUR personal/local tools

two types of MCPs
1> local MCP : allows AI to access tools and data on your local machine, providing a secure way to interact with your personal resources without exposing them to the internet.
2> remote MCP : allows AI to access tools and data hosted on remote servers, enabling integration with cloud-based services and APIs for enhanced functionality and scalability.

TAVILY searxch  - example of remote MCP 


HOOKS IN CLAUDE CODE:
Hooks are a powerful feature in Claude Code that allow you to execute custom code at specific points during the execution of your agentic graph.
Hooks = custom code that runs automatically when something happens.

They allow you to:
add validation
log activity
enforce rules
automate workflows
Hooks are used to control, monitor, or modify what happens automatically

Why do we need hooks?

Because without hooks:

👉 Everything happens as-is
👉 You have no control in between

>>preTool hook: runs before a tool is executed
>>postTool hook: runs after a tool is executed
