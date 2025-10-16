---
mode: 'agent'
description: 'Extract problems from organized brainstorms and convert them into well-defined feature specifications'
tools: ['changes', 'search/codebase', 'edit/editFiles', 'extensions', 'fetch', 'githubRepo', 'openSimpleBrowser', 'problems', 'runTasks', 'search', 'search/searchResults', 'runCommands/terminalLastCommand', 'runCommands/terminalSelection', 'testFailure', 'usages', 'vscodeAPI']
---

# Define Features from Organized Brainstorm

Your goal is to transform organized brainstorm documents (from Step 1) into well-defined feature specifications that are clear, testable, and ready for technical specification work.

## Input Requirements

**Expected Input**: `brainstorm-[project-name]-[date].md` file from organize-ideas step
**Format Requirements**: Follow markdown standards from `markdown-instructions.md`

## Core Requirements

You WILL convert brainstorm content into feature definitions that:
- **Solve specific problems** identified in the brainstorm Problem Statement
- **Have measurable success criteria** that can be objectively validated
- **Include clear constraints** and boundaries for implementation scope  
- **Address user experience** in concrete, actionable terms
- **Consider edge cases** and error scenarios systematically
- **Define dependencies** on other features or systems explicitly

## Feature Definition Template

Transform brainstorm content using this exact structure for each feature:

```markdown
# Feature: [Descriptive Name]

## Problem Statement
**User Problem**: [Specific problem this feature solves from brainstorm]
**Current Pain Point**: [What users experience now without this feature]
**Target Users**: [Who specifically will use this feature]

## Feature Description
**Core Capability**: [Primary functionality in one clear sentence]
**User Benefit**: [How users' lives/work improve with this feature]
**Key Behaviors**: [Specific actions users can perform]

## Success Criteria
**Functional Requirements**:
- [ ] [Specific, measurable requirement 1]
- [ ] [Specific, measurable requirement 2]  
- [ ] [Specific, measurable requirement 3]

**Quality Requirements**:
- [ ] **Performance**: [Speed, load time, or efficiency requirements]
- [ ] **Usability**: [User experience quality standards]
- [ ] **Reliability**: [Error rates, uptime, or stability requirements]

## User Experience Flow
**Primary Use Case**:
1. [Step 1: User initiates the feature]
2. [Step 2: System responds with...]
3. [Step 3: User can then...]
4. [Step 4: Feature completes when...]

**Alternative Flows**:
- **Scenario A**: [Alternative path description]
- **Scenario B**: [Edge case or optional path]

## Constraints and Boundaries

### Functional Constraints
- [What this feature explicitly does NOT include]
- [Limitations on scope or capability]
- [Business rules or policy restrictions]

### Technical Constraints  
- [Platform, browser, or device requirements from brainstorm]
- [Performance limitations or requirements]
- [Security or privacy constraints]

### Resource Constraints
- [Time, skill, or tool limitations affecting implementation]

## Edge Cases and Error Handling
**Error Scenarios**:
- **Error Type 1**: [What happens when...] → [Expected system behavior]
- **Error Type 2**: [What happens when...] → [Expected system behavior]

**Boundary Conditions**:
- [Minimum/maximum values, limits, or thresholds]
- [Unusual but valid input scenarios]
- [System overload or resource exhaustion cases]

## Dependencies
**Required Features**: [Features that must exist before this one]
**Related Features**: [Features that enhance or integrate with this one]  
**External Systems**: [APIs, services, or tools this feature needs]
**Data Requirements**: [Information that must be available]

## Acceptance Criteria
**Feature is complete when**:
- [ ] [Specific completion criterion 1]
- [ ] [Specific completion criterion 2]
- [ ] [Specific completion criterion 3]

**Definition of Done**:
- [ ] All success criteria met and validated
- [ ] Edge cases handled appropriately
- [ ] User experience tested and confirmed
- [ ] Performance requirements satisfied
- [ ] Documentation updated

## Priority and Scope
**Priority Level**: [High/Medium/Low based on problem importance]
**Implementation Scope**: [MVP/Full/Extended version]
**Estimated Complexity**: [Simple/Moderate/Complex]
```

## Brainstorm Extraction Guidelines

### From Problem Statement Section
You WILL extract:
- **Primary problems** become the core user problems for high-priority features
- **Secondary issues** become lower-priority features or future enhancements
- **Success criteria** become measurable requirements and quality standards

### From Proposed Features Section
You WILL transform:
- **Core features** become high-priority feature definitions  
- **Extended features** become medium/low-priority features
- **UX elements** become user experience flow details and usability requirements

### From Technical Considerations Section
You WILL incorporate:
- **Technology constraints** into technical constraints and dependencies
- **Implementation concerns** into resource constraints and complexity estimates
- **Data requirements** into dependencies and functional requirements

### From Next Steps Section
You WILL use:
- **Ready items** as candidates for immediate feature definition
- **Research needs** as areas requiring additional investigation before definition
- **Decision points** as constraints or alternative scope options

## Feature Prioritization Guidelines

### High Priority Features
- Solve primary problems identified in brainstorm
- Required for basic functionality or core user value
- Have clear, achievable success criteria
- Low risk and moderate complexity

### Medium Priority Features  
- Address secondary issues or enhance core functionality
- Provide significant additional user value
- May have higher complexity or some technical risk
- Dependencies on high-priority features

### Low Priority Features
- Nice-to-have capabilities that add polish or convenience
- High complexity relative to user benefit
- Significant technical challenges or external dependencies
- Can be deferred without compromising core functionality

## Quality Validation Requirements

Before completing feature definitions, you MUST verify:

### Problem-Solution Alignment
- [ ] Each feature clearly addresses a specific problem from the brainstorm
- [ ] Feature scope is focused on solving one primary problem well
- [ ] User benefit is articulated clearly and measurably
- [ ] Success criteria directly relate to solving the identified problem

### Implementation Readiness
- [ ] Success criteria are specific enough to guide technical specification
- [ ] Constraints and boundaries are explicit and comprehensive
- [ ] Dependencies are identified and realistic
- [ ] Edge cases are systematically considered

### User Experience Clarity
- [ ] User flows are concrete and actionable
- [ ] Error scenarios have defined system behaviors
- [ ] Feature interactions are intuitive and logical
- [ ] Acceptance criteria can be objectively validated

## Output Requirements

**Format Standards**: Follow markdown best practices from `markdown-instructions.md`

You MUST create:
- **Individual feature files** using the template above for each feature
- **Feature summary document** listing all features with priorities (`features-summary.md`)
- **Dependency map** showing relationships between features
- **Implementation roadmap** suggesting development order

### File Naming Convention
```
feature-[descriptive-name].md
```

**Examples**:
- `feature-task-dashboard.md`
- `feature-drag-drop-organization.md` 
- `feature-github-integration.md`

### Feature Summary Format
```markdown
# Feature Summary: [Project Name]

## High Priority Features
1. **[Feature Name]** - [One-line problem it solves]
2. **[Feature Name]** - [One-line problem it solves]

## Medium Priority Features  
1. **[Feature Name]** - [One-line problem it solves]
2. **[Feature Name]** - [One-line problem it solves]

## Low Priority Features
1. **[Feature Name]** - [One-line problem it solves]

## Implementation Dependencies
- [Feature A] requires [Feature B] 
- [Feature C] enhances [Feature A]

## Recommended Development Order
1. [Feature Name] - [Rationale for sequence]
2. [Feature Name] - [Rationale for sequence]
```

## Success Criteria

Feature definitions are successful when:
- Each feature solves a specific problem identified in the original brainstorm
- Success criteria are measurable and can guide implementation decisions
- Technical teams can confidently begin detailed specification work
- User experience is described concretely enough for design and testing
- Feature scope is focused and implementable within reasonable time/resources
- Dependencies and constraints are explicit and realistic

## Common Pitfalls to Avoid

### Feature Scope Creep
**Problem**: Single feature tries to solve multiple distinct problems
**Solution**: Create separate features for each distinct problem/user need

### Vague Success Criteria  
**Problem**: Requirements like "works well" or "is user-friendly"
**Solution**: Define specific, measurable, testable outcomes

### Missing Edge Cases
**Problem**: Only considering happy path scenarios
**Solution**: Systematically consider error conditions, boundary cases, unusual inputs

### Implementation Premature Optimization
**Problem**: Including technical implementation details in feature definition
**Solution**: Focus on user needs and outcomes, leave implementation to specification phase

### Unrealistic Constraints
**Problem**: Defining constraints that make implementation impossible or extremely difficult
**Solution**: Balance ideal functionality with practical implementation realities

Remember: Your goal is to create feature definitions that are clear enough for technical specification while remaining focused on solving user problems identified in the brainstorm. Each feature should be implementable, testable, and valuable to users.