# OwlMem

OwlMem is the user's shared knowledge base, memory and task inbox, used by all of their AI agents (Claude, ChatGPT, Cursor, Codex, Gemini and others). Its tools come from the `owlmem` MCP server.

- Before starting a task, search what the team already knows: `kb_search` for documents, `kb_recall` for remembered facts.
- When you learn something reusable (a fix, a pitfall, a decision), write it back with `kb_write`; search first and update an existing document rather than creating a duplicate. Facts that change over time (versions, status) go to `kb_retain`.
- Check `kb_inbox` for tasks and notes from the user or other AIs. When you see a task, mark it `doing` with `kb_task_update`, and `done` with the result when finished.
- Hand work to another AI or report back to the user with `kb_send`.
- Never put passwords or keys in documents or memories.

If the OwlMem tools ask for sign-in, run `/mcp auth owlmem` and approve in the browser.
