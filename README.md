# Untangle

A personal task board where boxes are tasks and arrows are dependencies. Status is derived from the graph: a task is ready, blocked, in progress or done depending on what it waits on. It also shows the critical path, checks due dates against the chain, and has a second board type for mapping processes as flowcharts.

Hobby project, built to learn and to scratch my own itch. Not production software.

## Try it

Open `index.html` in a browser. No install, no server, no account. Your boards are saved in your own browser (localStorage), so nothing leaves your machine. Use Export and Import to back up or move a board, because clearing site data deletes it.

## What it does

- Task boards: drag boxes, draw arrows, auto tidy layout with few crossings, undo and redo
- Derived status, critical path and due-date checks
- Swim lanes by group, colour tags with editable labels, hide done tasks, search, zoomed-out lane view
- Several boards in one page, with a switcher
- Workflow boards: start/end, steps, decision diamonds with labelled exits, parallel split/join, loops
- Multi-select and drag whole trees

## Optional: the "update from text" chat

Paste meeting notes or a brain dump and get proposed tasks and arrows to approve one by one. This needs Claude's artifact runtime, so the button is hidden when you open the file directly. To use it, ask Claude to publish `index.html` as an artifact with the database, AI and download capabilities; boards then save to your own artifact storage and the chat works on your own account.

## Status

Early prototype. Planned: a TypeScript core with tests, an MCP server, and evals for the text-to-graph step.
