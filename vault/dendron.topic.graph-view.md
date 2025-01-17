---
id: 587e6d62-3c5b-49b0-aedc-02f62f0448e6
title: Graph View
desc: ""
updated: 1623091870058
created: 1595120707814
stub: false
---

## Summary

-   Visualize the notes in your workspace in a graph view
-   Click on a node to open up the corresponding note in your workspace
-   Much faster startup times than the legacy note graph
    -   Scales to virtually any size graph

## Commands

### Show Note Graph V2

Launch the command bar (see [link](https://www.dendron.so/notes/401c5889-20ae-4b3a-8468-269def4b4865.html#launch-the-command-bar) for info): `> Dendron: Show Note Graph V2`

Click on a node to open up the corresponding note in your workspace.

The note graph currently only supports hierarchical note connections. Future versions of the graph will support linked note connections and the ability to add custom filters and styling to your graph.

## RFCs

-   [[7 Graph Rework|dendron.rfc.7-graph-rework]]

---

## Legacy Note Graph

Dendron provides support for graph view using a fork of the [markdown-links](https://marketplace.visualstudio.com/items?itemName=tchayen.markdown-links) extension.

The Dendron graph view is generated using our hierarchical index. It also shows different relationships than most of the graph views you're probably used to.

Instead of showing edges as links between nodes, Dendron edges are the hierarchical relationships between your notes. Think of it as a 20,000 foot view of the structure of your knowledge base.

Note that this command is not optimized for performance and you might notice slowdowns if you have more than a few hundred notes. If you are running into performance issues, please upvote this [issue](https://github.com/dendronhq/dendron/issues/107) to prioritize the performance work!

### Commands

#### Dendron: Show Note Graph

Launch the command bar (see [link](https://www.dendron.so/notes/401c5889-20ae-4b3a-8468-269def4b4865.html#launch-the-command-bar) for info): `> Dendron: Show Note Graph`

Show your note hierarchies visually in a graph.

![](https://foundation-prod-assetspublic53c57cce-8cpvgjldwysl.s3-us-west-2.amazonaws.com/assets/images/graph.show-notes.gif)

#### Dendron: Show Schema Graph

Launch the command bar (see [link](https://www.dendron.so/notes/401c5889-20ae-4b3a-8468-269def4b4865.html#launch-the-command-bar) for info): `> Dendron: Show Schema Graph`

Show your note schemas visually in a graph. Schemas will be labelled by their `title` attribute. If `title` is not set, default to its `id`.

![](https://foundation-prod-assetspublic53c57cce-8cpvgjldwysl.s3-us-west-2.amazonaws.com/assets/images/graphs.show-schema.gif)

#### Dendron: Sync Note Graph

Updates the note graph with most recent changes

#### Dendron: Sync Schema Graph

Updates the schema graph with most recent changes
