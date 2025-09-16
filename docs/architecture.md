# Architecture (Draft)

## Layers
- Core: Base abstractions (Component, RenderContext, Registry)
- Components: Individual reusable blocks
- Renderer: Orchestrates assembly → HTML output

## Data Flow (Planned)
Input JSON/YAML → Validation → Component Tree → Render Pipeline → Output HTML

## Open Questions
- Theming injection strategy
- Layout composition vs nested containers
- Extensibility via plugin hooks