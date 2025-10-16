---
mode: 'agent'
description: 'Check technical specifications to make sure they have everything needed to start coding'
tools: ['changes', 'codebase', 'edit/editFiles', 'extensions', 'fetch', 'githubRepo', 'openSimpleBrowser', 'problems', 'runTasks', 'search', 'searchResults', 'terminalLastCommand', 'terminalSelection', 'testFailure', 'usages', 'vscodeAPI']
---

# Validate My Technical Specification

Review my technical specification and check if it has everything I need to start coding confidently. Point out anything missing or unclear.

## Simple Validation Checklist

Check my specification for these essentials:

### The Basics
- [ ] **Clear goal** - Is it obvious what this feature does?
- [ ] **Data structure** - What information gets stored/used?
- [ ] **User interface** - What screens/interactions are needed?
- [ ] **Integration points** - What APIs or services does it use?

### The Details  
- [ ] **Error handling** - What happens when things go wrong?
- [ ] **Performance** - Any speed or scale requirements?
- [ ] **Security** - What data needs protection?
- [ ] **Testing** - How will I verify it works?

### Key Questions to Ask
- "Can I start coding from this spec?"
- "What happens when [error scenario]?"
- "Are there any missing technical details?"
- "What could block implementation?"
- **Entity relationships**: Are all data connections defined?
- **Data constraints**: Are validation rules and limits specified?
- **Data lifecycle**: How is information created, updated, deleted?
- **Data migration**: How does existing data integrate?
- **Data consistency**: How are integrity constraints maintained?

### Phase 3: Interface Specification Review
You WILL verify:
- **API completeness**: Are all required endpoints defined?
- **Input validation**: Are parameter constraints specified?
- **Output formats**: Are response structures documented?
- **Error responses**: Are failure modes and codes defined?
- **Authentication**: Are security requirements integrated?

### Phase 4: Implementation Feasibility Assessment
You WILL evaluate:
- **Technical risks**: What could prevent successful implementation?
- **Complexity assessment**: Is the approach appropriate for the problem?
- **Resource requirements**: Are skill and time estimates realistic?
## Simple Validation Format

Give me feedback like this:

```markdown
## Spec Check: [Feature Name]

### Ready to Code? [Yes/No/Maybe]

### What's Missing
- [List anything I need to add before I can start coding]

### Potential Issues  
- [Point out anything that might cause problems during implementation]

### Suggestions
- [Simple improvements to make the spec better]

### Bottom Line
[Can I start coding, or what do I need to fix first?]
```

Focus on practical implementation readiness, not perfect documentation.