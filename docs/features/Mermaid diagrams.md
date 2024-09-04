---
title: "Mermaid Diagrams"
tags:
  - feature/transformer
---

Quartz supports Mermaid which allows you to add diagrams and charts to your notes. Mermaid supports a range of diagrams, such as [flow charts](https://mermaid.js.org/syntax/flowchart.html), [sequence diagrams](https://mermaid.js.org/syntax/sequenceDiagram.html), and [timelines](https://mermaid.js.org/syntax/timeline.html). This is enabled as a part of [[Obsidian compatibility]] and can be configured and enabled/disabled from that plugin.

By default, Quartz will render Mermaid diagrams to match the site theme.

> [!warning]
> Wondering why Mermaid diagrams may not be showing up even if you have them enabled? You may need to reorder your plugins so that [[ObsidianFlavoredMarkdown]] is _after_ [[SyntaxHighlighting]].

## Syntax

To add a Mermaid diagram, create a mermaid code block.

````
```mermaid
sequenceDiagram
    Alice->>+John: Hello John, how are you?
    Alice->>+John: John, can you hear me?
    John-->>-Alice: Hi Alice, I can hear you!
    John-->>-Alice: I feel great!
```
````

```mermaid
flowchart TD

%% Nodes

    A("fab:fa-youtube <a rel="noopener" href="https://www.youtube.com/watch?v=T5Zthq-QR2A&amp" target="_blank">Starter Guide</a>")

    B("fab:fa-youtube <a rel="noopener" href="https://www.youtube.com/watch?v=rfQ_yGJ8QAQ&amp" target="_blank">Make Flowchart</a>")

    C("fa:fa-book-open <a rel="noopener" href="https://mermaid.js.org/syntax/flowchart.html" target="_blank">Learn More</a>")

    D{"Use the editor"}

    E(fa:fa-shapes Visual Editor)

    F("fa:fa-chevron-up Add node in toolbar")

    G("fa:fa-comment-dots AI chat")

    H("fa:fa-arrow-left Open AI in side menu")

    I("fa:fa-code Text")

    J(fa:fa-arrow-left Type Mermaid syntax)

  

%% Edge connections between nodes

    A --> B --> C --> D -- Build and Design --> E --> F

    D -- Use AI --> G --> H

    D -- Mermaid js --> I --> J

  

%% Individual node styling. Try the visual editor toolbar for easier styling!

    style E color:#FFFFFF, fill:#AA00FF, stroke:#AA00FF

    style G color:#FFFFFF, stroke:#00C853, fill:#00C853

    style I color:#FFFFFF, stroke:#2962FF, fill:#2962FF

  

%% You can add notes with two "%" signs in a row!
```


---
