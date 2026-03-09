**Subject:** [GAIR] What changes when AI works in your context

---

Week 7 of 10 - From browser to local: introducing agents

---

Remember the copy-paste loop from last week? You describe an analysis, the AI writes code, you paste it into your editor, hit an error (or unexpected output), copy that back, get revised code, try again. Chat window on one side, editor on the other, you in the middle doing the shuttling. Or you might be using AI to revise your writing in the same kind of loop, copying one paragraph after the other.

It works. But there's something inefficient about it beyond the tedium. The AI can't see your data, or the broader context of the project. It doesn't know your file structure, your variable names, your code style across files. Every time you start a new chat, you're re-explaining context the AI should already have. And every time you hit an error, you're acting as a messenger between two systems that could, in principle, talk to each other.

This week introduces tools that close that gap. They're usually called "coding agents" or "AI coding assistants," which is accurate but limited. They do write code. They can also do a lot of other things.

**What agents actually are**

An agent is an AI that can take actions in your environment. Instead of producing text in a chat window for you to copy somewhere, it reads your files, writes code, runs it, sees the errors, fixes them, and iterates - all without you shuttling anything back and forth. It works in your project folder, with your actual data and your actual file structure.

The simplest version of this is an AI-enhanced code editor. Tools like **Cursor**, **Windsurf**, or **GitHub Copilot** sit inside your editor and suggest code as you type, or let you describe what you want in plain language and generate code that fits your existing project. They see your open files and can read other files in your project to understand context.

More autonomous agents go further. **Claude Code**, **OpenAI Codex**, **Gemini CLI** and more open projects like **OpenCode** or **Kilo Code** are stand-alone tools that can plan multi-step tasks: read several files to understand a project, propose changes across multiple files, run code to test their changes, and iterate when something breaks. You describe what you want, and the agent figures out the steps. Think of the difference as: a code editor with AI is like having a capable assistant sitting next to you, while an autonomous agent is more like briefing a colleague and checking their work afterwards.

**"Coding agents" are general-purpose tools**

The name "coding agent" suggests something narrow, but these tools are useful for much more than writing code. Because they can read files, search through documents, and produce structured output, they're effective at tasks like:

- Summarising a folder of PDFs and identifying themes across them
- Extracting structured data from messy documents
- Organising research notes into a literature table
- Drafting methods sections based on your analysis scripts
- Reviewing a manuscript for internal consistency

What makes them different from a chat interface isn't just that they write code. It's that they have *context*. They can see your actual project, not a description of it. That makes their output more specific and more useful, though not necessarily more correct. They generate with more context, which helps - but the verification habits from the rest of this course still apply. One helpful addition (which we don't have time for in this course) is version control. If you use something like *git*, you can use that to keep track of what the AI did, and what you then changed, taking a snapshot of each turn.

**What this looks like in practice**

Say you have a folder with 20 interview transcripts and you want to identify common themes. In a chat interface, you'd upload them one by one (or a few at a time, depending on size limits), ask for themes, and manually combine the results. With an agent, you can point it at the folder and say "read all transcripts, identify recurring themes, and create a summary table with quotes and file references." It reads the files, processes them, and produces the output, referring to specific documents by name.

Or say you ran an analysis last week and want to try a different specification. Instead of re-explaining your data and approach from scratch, the agent reads your existing code, understands what you did, and modifies it. When the modified code produces an error, it reads the error, diagnoses the problem, and tries again. The iteration that took five rounds of copy-pasting in a chat might take thirty seconds.

This is genuinely useful. It's also genuinely risky if you stop paying attention, and that's the topic for Thursday.

**Open vs closed, local vs cloud**

With agents, the question of where your data goes becomes more concrete. When you use a chat interface, you choose what to paste in. When an agent has access to your project folder, it can potentially read anything in there.

Agents generally do not send files to a cloud server (especially not data files). Instead, the LLM in the cloud generates pieces of code like "show me the variable names in that dataset" and only the results are sent back to the LLM to come up with the next command, or with its answer. However, data does not stay private. They will often send the first few rows of a dataset, for instance, so that the LLM can understand what types of values it contains. So with agents, you are exposing potentially sensitive data.

One way around that is to work with local models that run on your computer. Unless you have a *much* better computer than I do, however, they are generally *much* less capable than state-of-the-art online models, so that this quickly becomes frustrating. Your university could host better models on a secure computing cluster, but that is still rare. So for now, you will usually have to consider what data you are willing to share, keep sensitive data out of the project folders, and pick a provider with a data usage policy that is in line with your needs.

Given the increasing commitment to open data, however, few of us will find ourselves in situations where none of our research data can be shared with a cloud provider. These services only receive fragments of your data, and most commit not to use it for training. If your data will be publicly available in a few months anyway, the practical risk is low. So while data protection matters, of course, it can also appear overwhelming when it is often just about maintaining data hygiene principles already included in your ethics application or data management plan - i.e. keeping identifiable data away from your analysis workflow.

**Getting started**

If you want to try an agent this week, it is worth investing a little bit of money to get the experience of working with a top model. While tools like **OpenCode** give you access to some free and many very cheap open source models, this is not going to give you a full sense of what is possible at the cutting edge. Paid subscriptions to Claude, ChatGPT or Gemini give you access to their coding agents, so if you have one it is worth using that - otherwise consider getting one for a trial month. Also, GitHub Copilot offers a fairly generous free tier including some usage of top models if you verify your student/academic status, and can then be used as an agent through tools like Visual Studio.

Setting up an agent for the first time can involve a few steps, especially if you're new to code editors or the command line. This week's [course notes](LINK) include links to setup resources for the most accessible options. If you get stuck, the FORRT Slack channel is a good place to ask.

## Try this: agent meets your project (10-15 min)

Pick a project folder you're comfortable sharing with an AI tool - something with data files, analysis scripts, notes, or documents.

1. Point the agent at your project folder.
2. Start with orientation: "What's in this project? Summarise the key files and what they do." See how well it understands your work without explanation.
3. Then try a real task. Some options:
   - Redo part of last week's analysis, but this time let the agent read your data and code directly instead of describing them in a chat
   - Ask it to find inconsistencies across documents (e.g., do your methods section and analysis script describe the same procedure?)
   - Ask it to extract structured information from a set of PDFs or notes
   - Ask it to create a presentation (specifying audience, context etc) based on your manuscript, including some presentation-style graphs created from your data
4. Note: what could the agent do that the chat workflow couldn't? Where did having your actual files make a difference?

**Journal prompt**

What surprised you about what the agent could or couldn't do? Where did the shift from chat to agent matter most? Where did it not matter at all?
