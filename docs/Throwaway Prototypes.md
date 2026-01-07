---
title: "Throwaway Prototypes - Detailed Guide"
description: "Comprehensive guide to Throwaway Prototypes: Quick exploration and validation in requirements gathering"
author: "Development Team"
date: "2024"
---

# Throwaway Prototypes: Quick Exploration and Validation

## Overview

**Throwaway Prototypes** (also known as **Rapid Prototypes** or **Exploratory Prototypes**) are quick, low-fidelity implementations created to explore requirements, validate concepts, test technical feasibility, or gather user feedback. Unlike evolutionary prototypes, these are intentionally discarded after serving their purpose of learning and clarification.

## Definition

Throwaway Prototypes are:
- **Quick implementations** built rapidly to explore ideas
- **Low-fidelity solutions** focusing on specific aspects
- **Temporary artifacts** discarded after learning
- **Exploratory tools** for requirements clarification
- **Risk reduction** mechanisms for technical validation

## Key Characteristics

### Rapid Development
- Built quickly (hours to days, not weeks)
- Minimal code quality requirements
- Focus on speed over perfection
- Quick iteration cycles

### Low Fidelity
- May lack error handling
- Incomplete functionality
- Simplified user interfaces
- Mock data or hardcoded values

### Purpose-Driven
- Created for specific learning objectives
- Focused on answering specific questions
- Targeted exploration of unknowns
- Clear success criteria

### Disposable
- Intentionally not production-ready
- Discarded after learning
- Not maintained or extended
- Code not reused in final product

## When to Use Throwaway Prototypes

### Requirements Exploration
- **Unclear Requirements**: When requirements are vague or ambiguous
- **User Needs Discovery**: Understanding what users actually want
- **Feature Validation**: Testing if a feature concept works
- **Workflow Exploration**: Understanding user workflows

### Technical Feasibility
- **Technology Evaluation**: Testing new technologies or frameworks
- **Performance Validation**: Checking if approach meets performance needs
- **Integration Testing**: Verifying third-party integrations
- **Architecture Exploration**: Testing architectural patterns

### Design Validation
- **UI/UX Concepts**: Testing interface designs
- **User Experience**: Validating user flows
- **Interaction Patterns**: Exploring interaction models
- **Visual Design**: Testing design concepts

### Risk Mitigation
- **High-Risk Features**: Validating risky technical approaches
- **Unknown Domains**: Exploring unfamiliar problem domains
- **Complex Algorithms**: Testing algorithm feasibility
- **Scalability Concerns**: Validating scalability assumptions

## Essential Elements of a Throwaway Prototype

### 1. Prototype Purpose & Objectives

**What to Document:**
- Primary question to answer
- Learning objectives
- Success criteria
- What will be validated

**How to Find This:**
- Review requirements documents for ambiguities
- Identify gaps in stakeholder understanding
- List technical unknowns from architecture discussions
- Extract questions from interviews and workshops

**Example:**
```markdown
**Purpose**: Validate if real-time collaboration is feasible with WebSocket technology
**Objective**: Determine if WebSocket can handle 100 concurrent users with <100ms latency
**Success Criteria**: 
  - WebSocket connection stable for 100 users
  - Message latency < 100ms
  - No connection drops during 1-hour test
```

### 2. Scope Definition

**What to Document:**
- What is included in the prototype
- What is explicitly excluded
- Boundaries and limitations
- Assumptions made

**How to Find This:**
- Define minimal feature set needed to answer questions
- Identify what can be mocked or hardcoded
- List dependencies that won't be implemented
- Document what will be simplified

**Example:**
```markdown
**In-Scope**:
  - WebSocket server implementation
  - Basic message broadcasting
  - Connection management
  - Latency measurement

**Out-of-Scope**:
  - User authentication
  - Message persistence
  - Error recovery
  - UI polish
  - Production deployment
```

### 3. Technical Approach

**What to Document:**
- Technologies and frameworks to use
- Architecture pattern
- Key components
- Integration points

**How to Find This:**
- Review [Tool Selection](./Tool%20Selection.md) documents
- Consult technical team for recommendations
- Research similar implementations
- Consider team expertise

**Example:**
```markdown
**Technology Stack**:
  - Backend: Node.js with Socket.io
  - Frontend: React with Socket.io-client
  - Testing: Artillery.io for load testing

**Architecture**:
  - Single WebSocket server
  - In-memory connection management
  - No database (mock data)

**Key Components**:
  - WebSocket server
  - Connection handler
  - Message broadcaster
  - Latency monitor
```

### 4. Implementation Plan

**What to Document:**
- Development steps
- Timeline (usually hours/days)
- Resources needed
- Dependencies

**How to Find This:**
- Break down into minimal viable steps
- Estimate time for each step
- Identify required skills
- List external dependencies

**Example:**
```markdown
**Steps**:
  1. Set up basic WebSocket server (2 hours)
  2. Implement connection handling (1 hour)
  3. Add message broadcasting (1 hour)
  4. Create simple client (2 hours)
  5. Load testing setup (2 hours)
  6. Run tests and measure (1 hour)

**Total Time**: ~9 hours
**Resources**: 1 developer with Node.js experience
```

### 5. Test Scenarios & Validation

**What to Document:**
- Test cases to run
- Metrics to measure
- Success/failure criteria
- Edge cases to explore

**How to Find This:**
- Define measurable success criteria
- List scenarios from requirements
- Identify performance benchmarks
- Consider failure modes

**Example:**
```markdown
**Test Scenarios**:
  1. Single user connection/disconnection
  2. 10 concurrent users sending messages
  3. 50 concurrent users
  4. 100 concurrent users (target)
  5. Message burst (100 messages/second)

**Metrics**:
  - Connection latency
  - Message delivery latency
  - Connection stability
  - Server CPU/memory usage

**Success Criteria**:
  - All scenarios pass
  - Latency < 100ms for 100 users
  - No connection drops
```

### 6. Findings & Learnings

**What to Document:**
- Results of prototype
- Answers to original questions
- Discovered issues
- Recommendations

**How to Find This:**
- Run tests and collect data
- Document observations
- Analyze results against criteria
- Formulate recommendations

**Example:**
```markdown
**Findings**:
  - WebSocket handles 100 users successfully
  - Average latency: 45ms (meets requirement)
  - Connection drops at 150+ users
  - Memory usage acceptable

**Learnings**:
  - Socket.io scales well for target load
  - Need connection pooling for >100 users
  - Message queuing needed for bursts

**Recommendations**:
  - Proceed with WebSocket approach
  - Implement connection pooling
  - Add message queue for production
```

### 7. Next Steps

**What to Document:**
- Decisions made based on prototype
- Actions to take forward
- What to include in final design
- What to discard

**How to Find This:**
- Review findings against objectives
- Make go/no-go decisions
- Plan integration into final design
- Update requirements based on learnings

**Example:**
```markdown
**Decisions**:
  - ✅ Use WebSocket for real-time features
  - ✅ Use Socket.io library
  - ⚠️ Add connection pooling for scale

**Actions**:
  - Update architecture document
  - Add connection pooling to design
  - Include message queue in requirements
  - Discard prototype code
```

## Complete Example: E-Commerce Search Feature Prototype

### Prototype Document

```markdown
# Throwaway Prototype: E-Commerce Search with Elasticsearch

## 1. Purpose & Objectives

**Primary Question**: Can Elasticsearch provide sub-second search results for 1 million products?

**Learning Objectives**:
  - Validate Elasticsearch performance with large dataset
  - Test search relevance and ranking
  - Measure query response times
  - Understand indexing requirements

**Success Criteria**:
  - Search results in < 500ms
  - Relevant results in top 10
  - Handles 100 queries/second
  - Index size manageable

## 2. Scope Definition

**In-Scope**:
  - Elasticsearch setup and configuration
  - Product data indexing (1M products)
  - Basic search queries (text search)
  - Relevance scoring
  - Performance measurement

**Out-of-Scope**:
  - User interface
  - Authentication
  - Product images
  - Faceted search
  - Search analytics
  - Production deployment

**Assumptions**:
  - Product data available in CSV format
  - Single Elasticsearch node sufficient for testing
  - English language only

## 3. Technical Approach

**Technology Stack**:
  - Elasticsearch 8.x
  - Python with elasticsearch-py library
  - Sample product dataset (1M records)

**Architecture**:
  - Single Elasticsearch instance
  - Python script for indexing
  - Python script for query testing
  - No application layer (direct Elasticsearch queries)

**Key Components**:
  - Index mapping definition
  - Data indexing script
  - Query testing script
  - Performance measurement tool

## 4. Implementation Plan

**Steps**:
  1. Set up Elasticsearch locally (30 min)
  2. Design index mapping (1 hour)
  3. Prepare sample data (1 hour)
  4. Index 1M products (2 hours)
  5. Create test queries (1 hour)
  6. Run performance tests (1 hour)
  7. Analyze results (1 hour)

**Total Time**: ~7.5 hours
**Resources**: 1 developer with Python and Elasticsearch basics

## 5. Test Scenarios & Validation

**Test Scenarios**:
  1. Simple text search: "laptop"
  2. Multi-word search: "wireless mouse"
  3. Partial match: "lap"
  4. Brand search: "apple"
  5. Category search: "electronics"
  6. Complex query: "gaming laptop under 1000"
  7. Load test: 100 queries/second

**Metrics**:
  - Query response time (p50, p95, p99)
  - Search relevance (manual review)
  - Index size
  - Memory usage
  - CPU usage

**Success Criteria**:
  - All queries < 500ms (p95)
  - Relevant results in top 10
  - Handles 100 qps without degradation
  - Index size < 5GB

## 6. Findings & Learnings

**Results**:
  - Average query time: 120ms ✅
  - P95 query time: 380ms ✅
  - P99 query time: 450ms ✅
  - Index size: 2.3GB ✅
  - Handles 100 qps: Yes ✅
  - Relevance: Good for simple queries, needs tuning for complex

**Discoveries**:
  - Default analyzer works well for English
  - Need custom analyzers for product names
  - Fuzzy matching needed for typos
  - Faceted search will require additional fields
  - Indexing time: ~30 minutes for 1M products

**Issues Found**:
  - Complex queries need relevance tuning
  - No support for typo tolerance out of box
  - Need to handle special characters

**Recommendations**:
  - ✅ Proceed with Elasticsearch
  - Add custom analyzers for product search
  - Implement fuzzy matching
  - Plan for faceted search fields
  - Consider search-as-you-type with completion suggester

## 7. Next Steps

**Decisions Made**:
  - ✅ Use Elasticsearch for product search
  - ✅ Implement custom analyzers
  - ✅ Add fuzzy matching
  - ✅ Plan faceted search architecture

**Actions**:
  - Update system design with Elasticsearch
  - Add search requirements to specification
  - Include custom analyzer configuration
  - Plan faceted search implementation
  - **Discard prototype code** (not production-ready)

**Updated Requirements**:
  - Search response time: < 500ms (validated)
  - Support fuzzy matching for typos
  - Custom analyzers for product names
  - Faceted search for filters
```

## How to Find Details for Each Element

### Finding Prototype Purpose & Objectives

**Sources:**
1. **Requirements Documents**: Look for ambiguous or unclear requirements
   - Search for words like "TBD", "to be determined", "explore", "investigate"
   - Identify requirements marked as "high risk" or "unknown"
   - Find features with question marks or uncertainty

2. **Stakeholder Interviews**: Extract questions and concerns
   - Review [Structured Interviews](./Structured%20Interviews.md) notes
   - Review [Unstructured Interviews](./Unstructured%20Interviews.md) transcripts
   - Look for phrases like "we're not sure if...", "we need to test...", "can we...?"

3. **Technical Discussions**: Identify technical unknowns
   - Architecture review meetings
   - Technology evaluation discussions
   - Performance requirement questions

4. **Risk Registers**: Find high-risk items needing validation
   - Review project risk documents
   - Identify technical risks
   - Find unproven technologies

**Tools:**
- **Document Analysis**: Use grep/search in requirements docs
- **Meeting Notes**: Review meeting transcripts or notes
- **Issue Trackers**: Check Jira/GitHub issues for questions
- **Brainstorming Sessions**: Capture questions during planning

**Practical Method:**
```bash
# Search requirements documents for uncertainties
grep -r "TBD\|to be determined\|explore\|investigate" docs/
grep -r "?" docs/requirements/
grep -r "unknown\|uncertain" docs/
```

### Finding Scope Definition

**Sources:**
1. **Requirements Prioritization**: Use MoSCoW or similar
   - Identify "Must Have" vs "Nice to Have"
   - Focus on core functionality only
   - Exclude non-essential features

2. **User Stories**: Break down to minimal viable
   - Extract core user journey
   - Remove edge cases
   - Simplify workflows

3. **Technical Architecture**: Identify minimal components
   - Core components only
   - Mock external dependencies
   - Skip non-critical integrations

**Tools:**
- **Requirements Management**: Jira, Azure DevOps, Trello
- **User Story Mapping**: Miro, Mural
- **Architecture Diagrams**: Draw.io, Lucidchart

**Practical Method:**
```markdown
1. List all features for the concept
2. Mark each as: Core / Supporting / Nice-to-Have
3. Include only "Core" in prototype
4. Document what's excluded and why
```

### Finding Technical Approach

**Sources:**
1. **Tool Selection Documents**: Review [Tool Selection](./Tool%20Selection.md)
   - Already evaluated technologies
   - Team expertise
   - Organizational standards

2. **Technology Research**: Quick research on options
   - Stack Overflow discussions
   - GitHub repositories
   - Official documentation

3. **Team Expertise**: Leverage team knowledge
   - Team skill assessment
   - Previous project experience
   - Technology preferences

**Tools:**
- **Technology Comparison**: StackShare, GitHub
- **Documentation**: Official docs, tutorials
- **Community**: Stack Overflow, Reddit, Discord
- **Proof of Concepts**: GitHub examples

**Practical Method:**
```markdown
1. List candidate technologies
2. Quick pros/cons for each
3. Check team familiarity
4. Select fastest to implement
5. Document decision rationale
```

### Finding Implementation Plan

**Sources:**
1. **Task Breakdown**: Decompose into small tasks
   - Setup tasks
   - Implementation tasks
   - Testing tasks
   - Analysis tasks

2. **Time Estimation**: Quick estimates
   - Use team velocity if available
   - Consider complexity
   - Add buffer for unknowns

3. **Resource Planning**: Identify needed skills
   - Required expertise
   - Team availability
   - External dependencies

**Tools:**
- **Task Management**: Jira, Trello, Asana
- **Time Tracking**: Toggl, Harvest
- **Planning**: Miro, Mural for breakdown

**Practical Method:**
```markdown
1. List all steps needed
2. Estimate each step (hours)
3. Identify dependencies
4. Sequence tasks
5. Total time estimate
```

### Finding Test Scenarios & Validation

**Sources:**
1. **Requirements**: Extract testable criteria
   - Performance requirements
   - Functional requirements
   - Quality attributes

2. **Success Criteria**: Define measurable outcomes
   - From prototype objectives
   - From requirements
   - From stakeholder expectations

3. **Risk Scenarios**: Test failure modes
   - What could go wrong?
   - Edge cases
   - Stress conditions

**Tools:**
- **Test Planning**: TestRail, Zephyr
- **Load Testing**: JMeter, Artillery, k6
- **Monitoring**: New Relic, Datadog (for production-like tests)

**Practical Method:**
```markdown
1. List success criteria
2. Convert to test scenarios
3. Define metrics to measure
4. Create test data
5. Plan test execution
```

### Finding Findings & Learnings

**Sources:**
1. **Test Results**: Collect data from tests
   - Performance metrics
   - Functional test results
   - Error logs
   - User feedback

2. **Observations**: Document what you see
   - Unexpected behaviors
   - Interesting patterns
   - Issues encountered

3. **Analysis**: Compare against criteria
   - Success vs failure
   - Performance vs targets
   - Issues vs expectations

**Tools:**
- **Data Collection**: Logs, metrics, screenshots
- **Analysis**: Spreadsheets, notebooks
- **Documentation**: Markdown, Confluence

**Practical Method:**
```markdown
1. Run all test scenarios
2. Collect metrics and logs
3. Document observations
4. Compare to success criteria
5. Identify patterns and issues
6. Formulate recommendations
```

### Finding Next Steps

**Sources:**
1. **Findings Analysis**: Based on prototype results
   - Go/no-go decisions
   - Design updates needed
   - Requirements changes

2. **Stakeholder Review**: Get input on findings
   - Present results
   - Get feedback
   - Make decisions

3. **Project Planning**: Integrate learnings
   - Update requirements
   - Update design
   - Update plan

**Tools:**
- **Decision Making**: Decision logs, meeting notes
- **Documentation**: Update requirements/design docs
- **Project Management**: Update tasks and plan

**Practical Method:**
```markdown
1. Review all findings
2. Make go/no-go decisions
3. List required changes
4. Update project documents
5. Plan next actions
6. Discard prototype
```

## Practical Tools for Creating Throwaway Prototypes

### Rapid Development Tools

#### Web Development Prototypes

**Frontend Frameworks:**
- **React + Vite**: Fast setup, hot reload
  ```bash
  npm create vite@latest prototype-name -- --template react
  ```
- **Vue.js + Vite**: Simple and fast
  ```bash
  npm create vite@latest prototype-name -- --template vue
  ```
- **Next.js**: Full-stack React, quick setup
  ```bash
  npx create-next-app@latest prototype-name
  ```

**Backend Prototypes:**
- **Express.js**: Minimal Node.js server
  ```bash
  npm init -y && npm install express
  ```
- **FastAPI (Python)**: Rapid API development
  ```bash
  pip install fastapi uvicorn
  ```
- **Flask (Python)**: Lightweight web framework
  ```bash
  pip install flask
  ```

**Full-Stack:**
- **Next.js**: React + API routes
- **SvelteKit**: Fast full-stack framework
- **Remix**: Full-stack React framework

#### Mobile Prototypes

**Cross-Platform:**
- **React Native**: Quick mobile apps
  ```bash
  npx react-native init PrototypeName
  ```
- **Flutter**: Fast development, single codebase
  ```bash
  flutter create prototype_name
  ```

**Native Quick Prototypes:**
- **SwiftUI (iOS)**: Rapid iOS development
- **Jetpack Compose (Android)**: Modern Android UI

#### Desktop Prototypes

- **Electron**: Web tech for desktop
  ```bash
  npm init electron-app@latest prototype-name
  ```
- **Tauri**: Lightweight alternative to Electron
- **Python + Tkinter**: Simple GUI prototypes

### Design & UI Tools

**Low-Fidelity Prototyping:**
- **Figma**: Interactive prototypes, fast iteration
- **Adobe XD**: UI/UX prototyping
- **Sketch**: Mac-based design tool
- **InVision**: Interactive prototypes

**Code-Based UI:**
- **Storybook**: Component development
  ```bash
  npx sb init
  ```
- **Tailwind CSS**: Rapid styling
  ```bash
  npm install -D tailwindcss
  ```

### Database & Data Tools

**Quick Database Setup:**
- **SQLite**: File-based, no setup
  ```python
  import sqlite3
  conn = sqlite3.connect('prototype.db')
  ```
- **PostgreSQL (Docker)**: Full-featured, containerized
  ```bash
  docker run --name pg-prototype -e POSTGRES_PASSWORD=test -d postgres
  ```
- **MongoDB (Docker)**: NoSQL, quick setup
  ```bash
  docker run --name mongo-prototype -d mongo
  ```

**Mock Data:**
- **Faker**: Generate fake data
  ```bash
  npm install faker
  # or
  pip install faker
  ```
- **JSON Generator**: Online mock data
- **Mockaroo**: Generate test data

### Testing & Validation Tools

**Load Testing:**
- **Artillery.io**: Node.js load testing
  ```bash
  npm install -g artillery
  artillery quick --count 100 --num 10 http://localhost:3000
  ```
- **k6**: Modern load testing
  ```bash
  brew install k6
  ```
- **Apache JMeter**: GUI-based load testing

**API Testing:**
- **Postman**: API testing and documentation
- **Insomnia**: API client
- **curl**: Command-line testing
  ```bash
  curl -X POST http://localhost:3000/api/test
  ```

**Performance Monitoring:**
- **Chrome DevTools**: Built-in performance tools
- **Lighthouse**: Web performance auditing
  ```bash
  npm install -g lighthouse
  lighthouse http://localhost:3000
  ```

### Documentation Tools

**Quick Documentation:**
- **Markdown**: Simple documentation
- **Notion**: Collaborative docs
- **Obsidian**: Knowledge base
- **Confluence**: Team documentation

**Code Documentation:**
- **JSDoc**: JavaScript documentation
- **Sphinx**: Python documentation
- **Swagger/OpenAPI**: API documentation

### Version Control

**Quick Git Setup:**
```bash
git init
git add .
git commit -m "Initial prototype"
```

**Branch Strategy for Prototypes:**
```bash
git checkout -b prototype/feature-name
# Work on prototype
# After learning, delete branch
git checkout main
git branch -D prototype/feature-name
```

## Practical Workflow: Step-by-Step

### Step 1: Identify Need for Prototype

**Activities:**
1. Review requirements for ambiguities
2. Identify technical unknowns
3. List high-risk items
4. Document questions to answer

**Output:** Prototype purpose document

**Time:** 1-2 hours

### Step 2: Define Scope

**Activities:**
1. List all potential features
2. Identify core vs supporting
3. Define what to exclude
4. Document assumptions

**Output:** Scope definition

**Time:** 30 minutes - 1 hour

### Step 3: Select Technology

**Activities:**
1. List candidate technologies
2. Quick evaluation (pros/cons)
3. Check team expertise
4. Select fastest option

**Output:** Technical approach document

**Time:** 1-2 hours

### Step 4: Create Implementation Plan

**Activities:**
1. Break into small tasks
2. Estimate each task
3. Sequence tasks
4. Identify resources

**Output:** Implementation plan

**Time:** 30 minutes - 1 hour

### Step 5: Build Prototype

**Activities:**
1. Set up development environment
2. Implement core functionality
3. Add minimal testing
4. Document as you go

**Output:** Working prototype

**Time:** 4-16 hours (depending on complexity)

### Step 6: Test & Validate

**Activities:**
1. Run test scenarios
2. Collect metrics
3. Document observations
4. Analyze results

**Output:** Test results and findings

**Time:** 2-4 hours

### Step 7: Document Learnings

**Activities:**
1. Summarize findings
2. Answer original questions
3. List recommendations
4. Update project documents

**Output:** Findings document

**Time:** 1-2 hours

### Step 8: Make Decisions & Clean Up

**Activities:**
1. Review findings with team
2. Make go/no-go decisions
3. Update requirements/design
4. Delete prototype code

**Output:** Updated project documents, discarded prototype

**Time:** 1-2 hours

**Total Time:** 10-30 hours (typically 1-3 days)

## Best Practices

### Do's

✅ **Keep it Simple**
- Focus on answering specific questions
- Don't build more than needed
- Use simplest technology that works

✅ **Time-Box It**
- Set strict time limits (hours/days, not weeks)
- Stop when you have answers
- Don't perfect the prototype

✅ **Document Everything**
- Document purpose and objectives
- Record findings immediately
- Capture decisions and rationale

✅ **Test Realistically**
- Use realistic data volumes
- Test actual use cases
- Measure real metrics

✅ **Involve Stakeholders**
- Show prototype to users
- Get feedback early
- Validate assumptions

### Don'ts

❌ **Don't Build Production Code**
- Prototype code should be discarded
- Don't optimize prematurely
- Don't add unnecessary features

❌ **Don't Skip Documentation**
- Document what you learn
- Record decisions made
- Share findings with team

❌ **Don't Extend Prototypes**
- Don't try to evolve into production
- Don't add features "just in case"
- Don't refactor prototype code

❌ **Don't Ignore Results**
- Use findings to make decisions
- Update requirements based on learnings
- Don't ignore negative results

❌ **Don't Take Too Long**
- Prototypes should be quick
- If taking weeks, it's not a throwaway prototype
- Reassess if timeline extends

## Common Pitfalls & How to Avoid Them

### Pitfall 1: Building Too Much

**Problem:** Prototype becomes too complex, takes too long

**Solution:**
- Strictly limit scope
- Remove features that don't answer core questions
- Set time limits and stick to them

### Pitfall 2: Trying to Reuse Code

**Problem:** Attempting to evolve prototype into production

**Solution:**
- Accept that code will be discarded
- Use learnings, not code
- Start fresh for production

### Pitfall 3: Not Testing Realistically

**Problem:** Testing with unrealistic data or scenarios

**Solution:**
- Use production-like data volumes
- Test actual use cases
- Measure real performance metrics

### Pitfall 4: Not Documenting Learnings

**Problem:** Knowledge lost when prototype is discarded

**Solution:**
- Document findings immediately
- Update requirements/design docs
- Share learnings with team

### Pitfall 5: Ignoring Negative Results

**Problem:** Dismissing results that don't support desired outcome

**Solution:**
- Accept and document all results
- Use negative results to pivot
- Make informed decisions based on data

## Integration with Requirements Gathering

Throwaway Prototypes are part of the requirements gathering process:

1. **Identify Gaps**: Prototypes reveal missing requirements
2. **Clarify Ambiguities**: Visual prototypes clarify vague requirements
3. **Validate Assumptions**: Test assumptions before committing
4. **Gather Feedback**: Get user input on concepts
5. **Reduce Risk**: Validate risky approaches early

See [Planning & Requirements Gathering](./Planning%20&%20Requirements%20Gathering.md) for the complete requirements process.

## Conclusion

Throwaway Prototypes are powerful tools for:
- **Exploring** unknown requirements
- **Validating** technical approaches
- **Reducing** project risk
- **Clarifying** ambiguous requirements
- **Learning** before committing

Key success factors:
- ✅ Clear purpose and objectives
- ✅ Strict scope and time limits
- ✅ Focus on learning, not building
- ✅ Document all findings
- ✅ Use learnings to inform decisions
- ✅ Discard prototype after learning

Remember: The value is in the **learning**, not the **code**. A successful throwaway prototype answers questions and reduces risk, even if the code is never used again.

