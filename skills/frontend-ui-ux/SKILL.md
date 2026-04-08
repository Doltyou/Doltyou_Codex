---
name: frontend-ui-ux
description: Designer-developer for UI/UX work
---

# Frontend UI/UX Command

Routes to the designer agent or Gemini MCP for frontend work.

## Usage

```
$frontend-ui-ux <design task>
```

## Routing

### Preferred: MCP Direct
Use available MCP tools directly when present; do not block on a separate discovery step if the runtime already exposes the needed tools.
Use a native subagent with role `designer` for focused UI/UX architecture or interaction-design passes when direct work is not enough.
If relevant MCP tools are unavailable, continue with the designer subagent fallback below.

### Fallback: Codex Agent
```
delegate(role="designer", tier="STANDARD", task="{{ARGUMENTS}}")
```

## Capabilities
- Component design and implementation
- Responsive layouts
- Design system consistency
- Accessibility compliance

Task: {{ARGUMENTS}}
