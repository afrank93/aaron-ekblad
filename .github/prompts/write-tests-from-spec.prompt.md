---
mode: 'agent'  
description: 'Generate comprehensive test cases from technical specifications for test-first development approach'
tools: ['changes', 'search/codebase', 'edit/editFiles', 'extensions', 'fetch', 'githubRepo', 'openSimpleBrowser', 'problems', 'runTasks', 'search', 'search/searchResults', 'runCommands/terminalLastCommand', 'runCommands/terminalSelection', 'testFailure', 'usages', 'vscodeAPI']
---

# Write Test Cases from Specifications

Your goal is to generate comprehensive test cases from technical specifications that validate all requirements and serve as acceptance criteria for test-driven development.

## Test Generation Framework

You WILL create test cases that cover:
- **Functional Requirements**: All specified capabilities and behaviors
- **Quality Requirements**: Performance, usability, reliability standards  
- **Edge Cases**: Boundary conditions and error scenarios
- **Integration Points**: Interfaces with other components or systems
- **User Experience Flows**: Complete interaction sequences
- **Security Requirements**: Authentication, authorization, data protection

## Test Case Structure Template

Generate test cases using this format for each specification:

```markdown
# Test Suite: [Feature Name]

*Generated from specification: [spec-file-name]*
*Test categories: Unit, Integration, End-to-End, Performance*

## Functional Requirement Tests

### Test Case: [Descriptive Name]
**Requirement**: [Specific requirement being tested from specification]
**Test Type**: [Unit/Integration/E2E]
**Setup**: [Initial conditions and test data needed]
**Actions**: 
1. [Step 1 - user action or system trigger]
2. [Step 2 - follow-up action]  
3. [Step 3 - validation action]
**Expected Results**:
- [Specific observable outcome 1]
- [Specific observable outcome 2]
**Acceptance Criteria**: [Pass/fail conditions from specification]

## Quality Requirement Tests

### Performance Test: [Performance Aspect]
**Requirement**: [Performance standard from specification]
**Test Type**: Performance/Load
**Test Conditions**: [Load parameters, data volume, concurrent users]
**Success Criteria**: [Specific timing/throughput requirements]
**Measurement Method**: [How performance will be measured]

### Usability Test: [User Experience Aspect]  
**Requirement**: [Usability standard from specification]
**Test Type**: Manual/Automated UI
**User Scenario**: [Realistic usage context]
**Success Criteria**: [Measurable usability outcomes]
**Validation Method**: [How usability will be confirmed]

## Edge Case and Error Tests

### Error Scenario: [Error Condition]
**Trigger**: [What causes this error condition]
**Expected Behavior**: [How system should respond from specification]
**Recovery Test**: [How system should return to normal operation]
**User Impact**: [What user experiences during error and recovery]

### Boundary Test: [Boundary Condition]
**Boundary**: [Minimum/maximum values or limits being tested]  
**Test Values**: [Specific values at and around boundaries]
**Expected Handling**: [How system should behave at boundaries]

## Integration Tests

### Integration Point: [System/Component Interface]
**Components**: [What systems/components are being integrated]
**Data Flow**: [Information exchange being tested]
**Success Criteria**: [Integration working correctly indicators]
**Failure Scenarios**: [What happens when integration fails]
```

## Test Case Generation Guidelines

### From Functional Requirements
You WILL create tests for:
- Every acceptance criterion listed in the specification
- All user actions and system responses described
- Data validation rules and business logic constraints  
- Component interactions and state changes
- API endpoints and their input/output contracts

### From Quality Requirements  
You WILL generate tests for:
- **Performance**: Response times, throughput, resource usage
- **Reliability**: Error rates, recovery procedures, data consistency
- **Usability**: Task completion times, learning curves, error prevention
- **Security**: Authentication, authorization, data protection measures

### From Edge Cases and Constraints
You WILL include tests for:
- **Input Boundaries**: Minimum, maximum, empty, invalid values
- **System Limits**: Capacity, concurrency, resource exhaustion  
- **External Dependencies**: Service unavailable, network failures, timeouts
- **User Errors**: Invalid operations, unexpected sequences, malformed inputs

## Test Prioritization Framework

### High Priority Tests (Must pass for release)
- Core functional requirements that solve primary user problems
- Critical user workflows and happy path scenarios
- Security requirements and data protection measures
- Integration points with external systems or critical components

### Medium Priority Tests (Should pass for quality)  
- Edge cases and error handling scenarios
- Performance requirements under normal load conditions
- Usability standards and user experience quality measures
- Non-critical integrations and optional features

### Low Priority Tests (Could defer if necessary)
- Stress testing beyond specified requirements  
- Usability edge cases and accessibility enhancements
- Performance optimization scenarios
- Extended error recovery procedures

## Test Implementation Guidance

### Unit Test Focus Areas
Generate unit tests for:
- Individual functions and methods with clear inputs/outputs
- Business logic validation and data transformation
- Component state management and lifecycle events
- Utility functions and helper methods

### Integration Test Focus Areas  
Generate integration tests for:
- API endpoints and data flow between services
- Database operations and data persistence
- External service integrations and error handling
- Component communication and event handling

### End-to-End Test Focus Areas
Generate E2E tests for:
- Complete user workflows from start to finish
- Cross-component functionality and user journeys  
- Real-world scenarios with realistic data and conditions
- Critical business processes and value delivery paths

## Test Data and Environment Requirements

### Test Data Strategy
You WILL specify:
- **Realistic Data Sets**: Representative of production usage patterns
- **Edge Case Data**: Boundary values, unusual but valid inputs
- **Invalid Data Sets**: For negative testing and error validation  
- **Performance Data**: Volume and variety appropriate for load testing

### Environment Configuration
You WILL define:
- **Test Environment Setup**: Dependencies, services, configuration required
- **Data Isolation**: How to prevent test interference and ensure repeatability
- **Cleanup Procedures**: Reset mechanisms between test runs
- **Monitoring Setup**: How to capture test results and performance metrics

## Success Criteria

Test suites are comprehensive when they:
- Cover all acceptance criteria from the original specification
- Include realistic user scenarios and workflows  
- Validate both success and failure behaviors systematically
- Provide clear pass/fail criteria that can be automated
- Enable confident release decisions based on test results
- Support test-driven development practices

## Quality Validation Requirements

Before finalizing test cases, verify:

### Coverage Completeness
- [ ] All functional requirements have corresponding test cases
- [ ] Quality requirements are measurably validated  
- [ ] Edge cases and error scenarios are systematically covered
- [ ] Integration points are thoroughly tested
- [ ] User experience flows are validated end-to-end

### Test Implementation Readiness  
- [ ] Test cases are specific enough to guide automation development
- [ ] Success criteria are objective and measurable
- [ ] Test data requirements are clearly specified
- [ ] Environment setup is documented and achievable
- [ ] Test execution sequence is logical and efficient

Remember: These test cases serve as both validation tools and acceptance criteria. They should be comprehensive enough to validate specification compliance while being practical to implement and maintain throughout development.