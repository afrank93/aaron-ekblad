---
mode: 'agent'
description: 'Create priority-ordered backlog from approved specifications based on dependencies, value, and risk'
tools: ['changes', 'search/codebase', 'edit/editFiles', 'extensions', 'fetch', 'githubRepo', 'openSimpleBrowser', 'problems', 'runTasks', 'search', 'search/searchResults', 'runCommands/terminalLastCommand', 'runCommands/terminalSelection', 'testFailure', 'usages', 'vscodeAPI']
---

# Prioritize Development Backlog

Your goal is to create a priority-ordered development backlog from approved technical specifications, considering dependencies, user value, learning goals, and implementation risk.

## Input Requirements

**Expected Input**: Technical specification files from Step 3 (`spec-[name].md` files from `/spec/` directory)
**Format Standards**: Follow markdown best practices from `markdown-instructions.md`

## Prioritization Framework

You WILL prioritize features using these weighted criteria:

### Value Assessment (40% weight)
- **User Impact**: How significantly does this improve user experience?
- **Problem Severity**: How painful is the current state without this feature?
- **Usage Frequency**: How often will users interact with this capability?
- **Business Value**: What organizational or efficiency gains does this provide?

### Dependency Analysis (30% weight)  
- **Hard Dependencies**: Features that must exist before this one can function
- **Soft Dependencies**: Features that enhance this one but aren't required
- **Enabling Value**: How many other features depend on this one?
- **Integration Complexity**: How many other systems or features are affected?

### Risk and Complexity (20% weight)
- **Technical Risk**: Likelihood of implementation challenges or blockers
- **Unknown Factors**: Areas requiring research or experimentation
- **Resource Requirements**: Skills, tools, or time investments needed
- **Alternative Approaches**: Availability of simpler solutions

### Learning and Strategic Value (10% weight)
- **Skill Development**: Opportunities to build important technical capabilities
- **Architecture Foundation**: Features that establish patterns for future work
- **Knowledge Building**: Learning that enables faster future development
- **Technology Exploration**: Valuable experience with new tools or approaches

## Backlog Structure Template

Create the prioritized backlog using this format:

```markdown
# Development Backlog: [Project Name]

*Prioritized: [Date]*
*Based on specifications: [List spec files analyzed]*

## Priority 1: Foundation Features (Implement First)
### [Feature Name] - [Estimated Effort: S/M/L]
**Value**: [Core user problem solved]
**Dependencies**: [None/List minimal dependencies]
**Risk**: [Low/Medium/High] - [Brief risk description]
**Rationale**: [Why this comes first - typically foundational, high value, low risk]

### [Feature Name] - [Estimated Effort: S/M/L]
[Same format for each Priority 1 feature]

## Priority 2: Core Functionality (Second Wave)
### [Feature Name] - [Estimated Effort: S/M/L]  
**Value**: [User benefit description]
**Dependencies**: [Features from Priority 1 required]
**Risk**: [Assessment with mitigation notes]
**Rationale**: [Why this priority level]

## Priority 3: Enhanced Experience (Third Wave)
### [Feature Name] - [Estimated Effort: S/M/L]
**Value**: [Additional user value provided]
**Dependencies**: [Previous features required]
**Risk**: [Risk level and considerations]
**Rationale**: [Why deferred to this priority]

## Priority 4: Advanced Features (Future Iterations)
### [Feature Name] - [Estimated Effort: S/M/L]
**Value**: [Nice-to-have benefits]  
**Dependencies**: [Complex dependency chains]
**Risk**: [High risk or complexity factors]
**Rationale**: [Why lowest priority - typically complex, high risk, or nice-to-have]

## Implementation Roadmap
### Milestone 1: [Timeline]
- [Priority 1 features that form coherent user value]
- **Goal**: [What user capability is achieved]
- **Success Criteria**: [How to validate milestone completion]

### Milestone 2: [Timeline]  
- [Priority 2 features building on Milestone 1]
- **Goal**: [Enhanced user capability achieved]
- **Success Criteria**: [Milestone validation criteria]

### Milestone 3: [Timeline]
- [Priority 3 features for complete experience]
- **Goal**: [Full feature experience achieved]  
- **Success Criteria**: [Complete feature set validation]

## Risk Mitigation Strategy
### High-Risk Features
- **[Feature Name]**: [Risk description] → [Mitigation approach]
- **[Feature Name]**: [Risk description] → [Mitigation approach]

### Dependency Chain Risks
- **If [Feature A] is blocked**: [Alternative approach or workaround]
- **If [Integration X] fails**: [Fallback strategy]

### Learning Investment Areas
- **[Technical Area]**: [Skills to develop] - [Learning timeline]
- **[Technology]**: [Knowledge needed] - [Research approach]
```

## Prioritization Decision Guidelines

### Priority 1 Criteria (Must implement first)
- Solves core user problems identified in original brainstorm
- Has minimal dependencies on other features  
- Low to medium technical risk
- Provides foundational architecture for future features
- Essential for basic user value proposition

### Priority 2 Criteria (Core functionality)
- Significantly enhances user experience beyond basics
- Depends on Priority 1 features but not complex chains
- Moderate risk with clear mitigation strategies
- High user value relative to implementation effort
- Completes primary user workflows

### Priority 3 Criteria (Enhanced experience)
- Improves user experience quality and efficiency
- May have complex dependencies but clear implementation path
- Medium to high risk but with acceptable fallback options
- Good user value but not essential for core functionality
- Enables advanced user capabilities

### Priority 4 Criteria (Future iterations)
- Nice-to-have features that add polish or convenience
- Complex dependency chains or high technical risk
- Significant implementation effort relative to user benefit
- Experimental or exploratory features
- Can be deferred without compromising core value

## Quality Validation Requirements

Before finalizing prioritization, verify:

### Value Alignment  
- [ ] Priority 1 features solve the most critical user problems from brainstorm
- [ ] Each priority level provides coherent user value
- [ ] Features within priority levels can be implemented in flexible order
- [ ] Milestone goals align with original project objectives

### Dependency Accuracy
- [ ] All hard dependencies are identified and correctly sequenced
- [ ] Circular dependencies are eliminated or broken
- [ ] Dependency chains don't exceed 3 levels deep
- [ ] Alternative approaches exist for high-risk dependencies

### Risk Assessment
- [ ] Technical risks are realistically evaluated
- [ ] Mitigation strategies are specific and actionable  
- [ ] High-risk features have fallback options
- [ ] Learning investments are sized appropriately

### Implementation Feasibility
- [ ] Priority 1 features are implementable with current skills/tools
- [ ] Effort estimates account for complexity and unknowns
- [ ] Milestone timelines are realistic for available resources
- [ ] Roadmap allows for iteration and course correction

## Success Criteria

The prioritized backlog is successful when:
- Development can begin immediately with Priority 1 features
- Each milestone delivers coherent user value
- Risk is front-loaded with mitigation strategies
- Dependencies enable rather than block progress
- Learning goals are integrated with delivery goals
- Features can be implemented in priority order without major rework

## Common Prioritization Pitfalls

### Avoid Perfect Dependency Ordering
**Problem**: Waiting for complete dependency analysis before starting
**Solution**: Start with clearly independent features, refine dependencies iteratively

### Avoid Risk Avoidance  
**Problem**: Deferring all challenging features to later priorities
**Solution**: Balance risk across priorities, front-load learning where possible

### Avoid Feature Perfectionism
**Problem**: Including too many features in early priorities
**Solution**: Focus on minimum viable functionality for each priority level

### Avoid Scope Creep
**Problem**: Adding new features during prioritization
**Solution**: Stick to features from approved specifications, document new ideas for future cycles

Remember: The goal is a workable development sequence that delivers user value incrementally while managing risk and dependencies. Perfect prioritization is less important than starting development with clear, implementable features.