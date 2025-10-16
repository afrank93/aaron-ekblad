---
mode: 'agent'
description: 'Convert prioritized specifications into well-structured GitHub issues ready for development work'
tools: ['changes', 'search/codebase', 'edit/editFiles', 'extensions', 'fetch', 'githubRepo', 'openSimpleBrowser', 'problems', 'runTasks', 'search', 'search/searchResults', 'runCommands/terminalLastCommand', 'runCommands/terminalSelection', 'testFailure', 'usages', 'vscodeAPI']
---

# Create GitHub Issues from Specifications

Your goal is to convert prioritized technical specifications into well-structured GitHub issues that provide clear work units for development with proper labeling, milestone assignment, and actionable acceptance criteria.

## GitHub Issue Structure Template

Transform specifications into issues using this format:

```markdown
# [Feature Name]: [Specific User Capability]

## Description
[Clear, concise explanation of what this feature accomplishes for users]

**User Problem**: [Specific problem this solves from original brainstorm]
**User Benefit**: [How users' workflow improves with this feature]

## Acceptance Criteria
- [ ] [Specific, testable requirement 1]
- [ ] [Specific, testable requirement 2]  
- [ ] [Specific, testable requirement 3]
- [ ] [Performance requirement with measurable target]
- [ ] [Error handling requirement for main edge cases]

## Technical Requirements
**Architecture**: [Component structure and integration points]
**Data Model**: [Key entities and relationships required]
**API Endpoints**: [Required interfaces with input/output specifications]
**Dependencies**: [Other features or external systems required]

## User Experience Requirements  
**Primary Flow**:
1. [User action that initiates feature]
2. [System response and user feedback]
3. [Follow-up user actions available]
4. [Completion state and user confirmation]

**Error Handling**: [How errors are presented to users]
**Performance**: [User-visible speed requirements]

## Implementation Notes
**Suggested Approach**: [Recommended technical implementation strategy]
**Risk Factors**: [Technical challenges to be aware of]
**Testing Strategy**: [Key areas to validate during development]

## Definition of Done
- [ ] All acceptance criteria verified and passing
- [ ] User experience tested and confirmed intuitive  
- [ ] Performance requirements met under test conditions
- [ ] Edge cases handled gracefully with appropriate user feedback
- [ ] Integration with dependent features validated
- [ ] Code reviewed and meets project quality standards
- [ ] Documentation updated for any new interfaces or configuration

## Labels
`[priority-high/medium/low]` `[type-feature]` `[milestone-v1.0]` `[component-frontend/backend/api]`

## Estimated Effort  
**Size**: [Small (1-3 days) / Medium (4-7 days) / Large (1-2+ weeks)]
**Complexity**: [Low/Medium/High]
**Dependencies**: [List of blocking issues or external requirements]
```

## Issue Creation Guidelines

### Title Format Standards
Use this pattern for consistent issue titles:
- **Feature Issues**: `[Component] Feature: [User Capability]`
- **Bug Issues**: `[Component] Bug: [Problem Description]`  
- **Technical Issues**: `[Component] Tech: [Technical Improvement]`

**Examples**:
- `Dashboard Feature: Task Status Overview with Filtering`
- `Authentication Feature: User Login with Session Management`
- `API Feature: GitHub Integration for Issue Import`

### Description Writing Standards
You WILL write descriptions that:
- Start with user-focused problem and benefit statements
- Avoid technical jargon in the main description
- Clearly connect to original brainstorm problems
- Explain the value proposition for end users

### Acceptance Criteria Standards  
You WILL create criteria that are:
- **Specific**: No ambiguous language like "works well" or "user-friendly"
- **Testable**: Can be objectively verified as complete or incomplete
- **Complete**: Cover all aspects of the specification requirement
- **Measurable**: Include quantitative targets where specified

**Good Examples**:
- `User can filter tasks by project, status, and due date with results updating in <2 seconds`
- `Dashboard displays all tasks from connected sources with real-time status updates`
- `Error messages appear within 3 seconds of invalid input with specific guidance for correction`

**Avoid**:
- `Dashboard works well for users`
- `Filtering is intuitive and responsive`  
- `Error handling is comprehensive`

## Labeling and Organization Standards

### Required Labels
Every issue MUST include:
- **Priority**: `priority-high`, `priority-medium`, `priority-low`
- **Type**: `type-feature`, `type-bug`, `type-tech-debt`, `type-documentation`  
- **Milestone**: `milestone-v1.0`, `milestone-v1.1`, etc.
- **Component**: `component-frontend`, `component-backend`, `component-api`, `component-database`

### Optional Enhancement Labels
Use when appropriate:
- **Effort**: `effort-small`, `effort-medium`, `effort-large`
- **Skill**: `skill-frontend`, `skill-backend`, `skill-design`, `skill-devops`
- **Status**: `status-blocked`, `status-in-progress`, `status-review`
- **Special**: `good-first-issue`, `help-wanted`, `breaking-change`

### Milestone Assignment Guidelines
- **v1.0 (MVP)**: Priority 1 features that provide core user value
- **v1.1 (Enhanced)**: Priority 2 features that improve user experience  
- **v1.2 (Advanced)**: Priority 3 features that add polish and convenience
- **Future**: Priority 4 features deferred to later versions

## Issue Relationships and Dependencies

### Dependency Documentation
You WILL document dependencies by:
- **Blocking Issues**: Use GitHub's "blocked by" relationships
- **Related Issues**: Link to complementary or enhancing features  
- **Parent/Child**: Break large features into smaller, implementable issues
- **External Dependencies**: Note third-party services, APIs, or tools required

### Epic and Story Organization  
For complex features:
- **Epic Issue**: High-level feature description with user value proposition
- **Story Issues**: Specific implementable components of the epic
- **Task Issues**: Technical work items that support story completion

**Example Structure**:
- Epic: `Task Management Dashboard`  
  - Story: `Basic Task Display with Status`
  - Story: `Task Filtering and Search`  
  - Story: `Drag-Drop Task Organization`

## Issue Quality Validation

### Completeness Check
Before creating issues, verify:
- [ ] All specification requirements are covered by acceptance criteria
- [ ] User experience is described concretely with specific flows
- [ ] Technical requirements provide implementation guidance
- [ ] Dependencies on other issues or systems are identified
- [ ] Effort estimation is realistic based on scope and complexity

### Clarity Check  
Ensure issues are actionable:
- [ ] Developer can understand what to build from description and criteria
- [ ] Success conditions are objectively measurable
- [ ] Technical approach provides sufficient implementation direction
- [ ] Definition of done covers all aspects of feature completion

### Workflow Integration Check
Verify issues support development workflow:
- [ ] Issues are sized appropriately for sprint planning (1-2 weeks maximum)
- [ ] Dependencies allow for parallel development where possible  
- [ ] Priority and milestone assignments align with project roadmap
- [ ] Labels support filtering and progress tracking needs

## Success Criteria

GitHub issues are ready for development when:
- Developers can confidently estimate effort and begin implementation
- Acceptance criteria provide clear success conditions for testing
- Dependencies are identified and can be managed in sprint planning
- User value is obvious and connects to original project goals
- Technical guidance is sufficient for architecture and implementation decisions
- Quality standards are explicit and measurable

## Common Issue Creation Pitfalls

### Avoid Vague Acceptance Criteria
**Problem**: Criteria like "users find it intuitive" or "performs well"
**Solution**: Replace with specific, measurable outcomes like "new users complete setup in <5 minutes"

### Avoid Technical Implementation Details in Description  
**Problem**: Leading with database schema or API design in main description
**Solution**: Start with user problem and benefit, put technical details in implementation notes

### Avoid Overly Large Issue Scope
**Problem**: Issues that take multiple weeks or cover multiple distinct features
**Solution**: Break into smaller, implementable pieces that deliver incremental value

### Avoid Missing Dependency Documentation  
**Problem**: Issues that seem independent but actually require other features
**Solution**: Explicitly identify and link all blocking relationships and external dependencies

Remember: GitHub issues serve as the bridge between specifications and implementation. They should provide developers with clear, actionable work units that deliver measurable progress toward the original project goals.