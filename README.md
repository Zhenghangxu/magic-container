This is a WIP project exploring the topic of end-to-end UI generation using the power of LLM


## Preliminary Research

### Any existing solutions?
- Vercel V0

### TechStacks (Work in Progress)

#### LLM
#### UI Libraries
Radix UI / Shadcn
#### DB (for context and caching)
#### External Connectors 

### Pipeline (Work in Progress)
flowchart TD
    A[Prompt] --> B(extract data/style requirement from prompt)
    B --> C{Routing Agent}
    C -->|Data:JSON schema| D[Similarity Search on existing Components schema] --> G{match?}
    C --> P[Generate Layout] --Theme --> E{Is stylized?}
    G -->|yes| H[rewrite schema]
    G -->|no| I(new component)
    E -->|yes| J(Generate Base Design:Stable Diffusion)
    E -->|no| K(Generate CSS code)
    
---

### Agents

#### Data Converters

#### Layout Genenerator

#### Painter

#### UI Code Generators

#### Testers


---

### UI Generation

#### Brand-agnotic

#### How to handle highly-stylized elements?
- animation
- custom artwork
- unconventional layout etc.

#### Mantainability
- Human readable source code

#### UX/UI
- Automated Accessibility
- AI agent for usability testing?

#### Updating UI with prompt?

### Generate in client with Transformer.js?