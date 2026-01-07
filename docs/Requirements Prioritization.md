---
title: "Requirements Prioritization - Detailed Guide"
description: "Comprehensive guide to Requirements Prioritization: Methods, techniques, and tools for prioritizing requirements"
author: "Development Team"
date: "2024"
---

# Requirements Prioritization: Methods, Techniques, and Tools

## Overview

**Requirements Prioritization** is the process of ranking requirements in order of importance, value, or urgency to guide development efforts. It helps teams focus on delivering the most valuable features first, manage limited resources effectively, and make informed decisions about what to build and when.

## Definition

Requirements Prioritization is:
- **Ranking process** that orders requirements by importance
- **Decision-making framework** for resource allocation
- **Value optimization** to maximize business impact
- **Risk management** to address critical needs first
- **Scope management** to balance needs and constraints

## Key Characteristics

### Value-Driven
- Focus on business value
- Maximize ROI
- Align with business objectives
- Prioritize high-impact features

### Stakeholder-Centric
- Involves key stakeholders
- Balances different perspectives
- Manages expectations
- Ensures buy-in

### Evidence-Based
- Uses data and analysis
- Considers multiple factors
- Objective evaluation
- Measurable criteria

### Dynamic Process
- Re-evaluated regularly
- Adapts to changes
- Responds to feedback
- Iterative refinement

## Why Prioritize Requirements?

### Resource Constraints
- Limited development capacity
- Budget limitations
- Time constraints
- Team availability

### Business Value
- Maximize ROI
- Deliver value early
- Meet critical deadlines
- Achieve business objectives

### Risk Management
- Address high-risk items early
- Validate assumptions
- Reduce project risk
- Manage dependencies

### Stakeholder Management
- Manage expectations
- Balance competing needs
- Ensure alignment
- Build consensus

## Prioritization Methods

### 1. MoSCoW Method

**Definition**: Categorizes requirements into Must Have, Should Have, Could Have, and Won't Have.

**Categories**:
- **Must Have (M)**: Critical, cannot launch without
- **Should Have (S)**: Important, but not critical
- **Could Have (C)**: Nice to have, low priority
- **Won't Have (W)**: Out of scope (for now)

**Best For**: Clear categorization, stakeholder communication

**Limitations**: Can be subjective, may have too many "Must Haves"

### 2. Value vs. Effort Matrix

**Definition**: Plots requirements on a 2x2 matrix based on value and effort.

**Quadrants**:
- **Quick Wins**: High value, low effort (do first)
- **Major Projects**: High value, high effort (plan carefully)
- **Fill-ins**: Low value, low effort (do if time permits)
- **Time Sinks**: Low value, high effort (avoid)

**Best For**: Visual prioritization, resource optimization

**Limitations**: Value and effort can be subjective

### 3. Kano Model

**Definition**: Categorizes features based on customer satisfaction.

**Categories**:
- **Basic (Must-Be)**: Expected features, dissatisfaction if missing
- **Performance (One-Dimensional)**: More is better, linear satisfaction
- **Delight (Attractive)**: Unexpected features, high satisfaction

**Best For**: Understanding customer satisfaction, feature categorization

**Limitations**: Requires customer research, can be complex

### 4. Priority Scoring

**Definition**: Assigns numerical scores based on multiple criteria.

**Criteria Examples**:
- Business value (1-10)
- User impact (1-10)
- Technical risk (1-10)
- Dependencies (1-10)
- Cost/Effort (1-10)

**Best For**: Objective prioritization, complex requirements

**Limitations**: Can be time-consuming, requires consensus on criteria

### 5. Weighted Shortest Job First (WSJF)

**Definition**: Prioritizes based on cost of delay divided by job duration.

**Formula**: WSJF = Cost of Delay / Job Duration

**Cost of Delay Factors**:
- User/business value
- Time criticality
- Risk reduction
- Opportunity enablement

**Best For**: Agile/SAFe environments, maximizing value delivery

**Limitations**: Requires accurate estimates, can be complex

### 6. RICE Scoring

**Definition**: Scores features using Reach, Impact, Confidence, and Effort.

**Formula**: RICE = (Reach × Impact × Confidence) / Effort

**Components**:
- **Reach**: How many users affected (per time period)
- **Impact**: Impact per user (0.25, 0.5, 1, 2, 3)
- **Confidence**: Confidence in estimates (50%, 80%, 100%)
- **Effort**: Person-months of work

**Best For**: Product management, feature prioritization

**Limitations**: Requires data, can be time-consuming

### 7. Business Value Points

**Definition**: Assigns business value points to requirements.

**Scoring**:
- Critical business value: 9 points
- High business value: 6 points
- Medium business value: 3 points
- Low business value: 1 point

**Best For**: Business-focused prioritization

**Limitations**: May not consider technical factors

### 8. Dependency-Based Prioritization

**Definition**: Prioritizes based on requirement dependencies.

**Approach**:
- Identify dependencies
- Prioritize foundational requirements
- Build dependent requirements after
- Consider critical path

**Best For**: Technical requirements, architecture dependencies

**Limitations**: May not optimize for business value

## Essential Elements of Requirements Prioritization

### 1. Requirement Information

**What to Document:**
- Requirement ID
- Requirement name/description
- Requirement type (Functional, NFR, etc.)
- Source/stakeholder
- Current priority

**How to Find This:**
- Review requirements documents
- Check [Functional Requirements](./Functional%20Requirements.md)
- Check [Non-Functional Requirements](./Non-Functional%20Requirements.md)
- Review [Business Requirements](./Business%20Requirements.md)
- Check requirements management tools

**Example:**
```markdown
**Requirement ID**: FR-045
**Name**: User Authentication
**Type**: Functional Requirement
**Source**: Security Team, Product Owner
**Current Priority**: Must Have (M)
**Description**: System shall allow users to authenticate using email and password
```

### 2. Prioritization Criteria

**What to Document:**
- Criteria used for prioritization
- Weight/importance of each criterion
- Scoring scale
- Evaluation method

**How to Find This:**
- Define based on business objectives
- Review [Project Charter](./Project%20Charter.md) for goals
- Consult stakeholders for priorities
- Consider project constraints
- Review industry best practices

**Example:**
```markdown
**Prioritization Criteria**:
  1. Business Value (Weight: 30%)
     - Critical to business objectives: 10 points
     - Important to business: 7 points
     - Nice to have: 3 points
     - Low value: 1 point

  2. User Impact (Weight: 25%)
     - Affects all users: 10 points
     - Affects majority: 7 points
     - Affects some users: 4 points
     - Affects few users: 1 point

  3. Technical Risk (Weight: 20%)
     - Low risk, proven technology: 10 points
     - Medium risk: 6 points
     - High risk, unproven: 2 points

  4. Dependencies (Weight: 15%)
     - No dependencies: 10 points
     - Few dependencies: 7 points
     - Many dependencies: 3 points
     - Blocks other work: 1 point

  5. Effort/Cost (Weight: 10%)
     - Low effort (< 1 week): 10 points
     - Medium effort (1-4 weeks): 6 points
     - High effort (> 4 weeks): 2 points
```

### 3. Stakeholder Input

**What to Document:**
- Stakeholders involved
- Their priorities/ratings
- Consensus or conflicts
- Decision rationale

**How to Find This:**
- Conduct prioritization workshops
- Survey stakeholders
- Review stakeholder interviews
- Check [Structured Interviews](./Structured%20Interviews.md)
- Review [Unstructured Interviews](./Unstructured%20Interviews.md)
- Hold voting sessions

**Example:**
```markdown
**Stakeholders Involved**:
  - Product Owner: John Smith
  - Technical Lead: Sarah Johnson
  - Business Analyst: Mike Davis
  - Security Lead: Lisa Chen
  - End User Representative: Tom Wilson

**Stakeholder Ratings** (1-10 scale):
  FR-045 (User Authentication):
    - Product Owner: 9 (Critical for launch)
    - Technical Lead: 8 (Foundation for other features)
    - Business Analyst: 9 (Core requirement)
    - Security Lead: 10 (Security requirement)
    - End User: 7 (Necessary but expected)
    Average: 8.6

**Consensus**: High - All stakeholders agree this is critical
**Conflicts**: None
**Decision**: Must Have (M) - Approved by all stakeholders
```

### 4. Scoring & Ranking

**What to Document:**
- Scores for each criterion
- Weighted scores
- Total priority score
- Final ranking
- Priority category

**How to Find This:**
- Calculate scores based on criteria
- Apply weights
- Sum weighted scores
- Rank by total score
- Assign priority category

**Example:**
```markdown
**Scoring for FR-045 (User Authentication)**:

  Business Value: 10 points × 30% = 3.0
  User Impact: 10 points × 25% = 2.5
  Technical Risk: 8 points × 20% = 1.6
  Dependencies: 10 points × 15% = 1.5
  Effort/Cost: 6 points × 10% = 0.6
  ------------------------------------
  Total Score: 9.2 / 10.0

**Ranking**: #1 (Highest priority)
**Priority Category**: Must Have (M)
**Justification**: Critical for security and enables other features
```

### 5. Dependencies & Relationships

**What to Document:**
- Requirements this depends on
- Requirements that depend on this
- Blocking relationships
- Critical path items

**How to Find This:**
- Review requirement relationships
- Analyze architecture dependencies
- Check technical dependencies
- Review functional dependencies
- Map requirement traceability

**Example:**
```markdown
**Dependencies for FR-045 (User Authentication)**:

  **Depends On**:
    - NFR-002: Security requirements (encryption, etc.)
    - FR-001: User registration (must register before login)
    - NFR-010: Infrastructure (authentication service)

  **Enables**:
    - FR-046: User profile management
    - FR-047: Access control
    - FR-048: User preferences
    - FR-049: Order history

  **Blocks**: None (foundational requirement)

  **Critical Path**: Yes - Many features depend on this
  **Impact**: High - Delaying this blocks 15+ other requirements
```

### 6. Risk Assessment

**What to Document:**
- Technical risks
- Business risks
- Schedule risks
- Resource risks
- Risk mitigation

**How to Find This:**
- Review risk registers
- Analyze technical complexity
- Assess business impact of delay
- Consider resource availability
- Evaluate schedule constraints

**Example:**
```markdown
**Risk Assessment for FR-045 (User Authentication)**:

  **Technical Risks**:
    - Risk: Integration with SSO providers may be complex
    - Probability: Medium
    - Impact: High
    - Mitigation: Use proven authentication library (Auth0)

  **Business Risks**:
    - Risk: Security breach if not implemented correctly
    - Probability: Low (with proper implementation)
    - Impact: Critical
    - Mitigation: Security review, penetration testing

  **Schedule Risks**:
    - Risk: May delay other dependent features
    - Probability: Medium
    - Impact: High
    - Mitigation: Prioritize early, allocate experienced developers

  **Overall Risk Level**: Medium-High
  **Risk Justification**: High impact if delayed, but manageable with proper planning
```

### 7. Business Value Analysis

**What to Document:**
- Business value score
- Revenue impact
- Cost savings
- Strategic alignment
- Competitive advantage

**How to Find This:**
- Review [Business Requirements](./Business%20Requirements.md)
- Analyze business objectives
- Review [Project Charter](./Project%20Charter.md)
- Consult business stakeholders
- Estimate financial impact

**Example:**
```markdown
**Business Value Analysis for FR-045 (User Authentication)**:

  **Business Value Score**: 10/10 (Critical)

  **Revenue Impact**:
    - Enables user accounts and personalized experience
    - Required for e-commerce transactions
    - Estimated revenue impact: $500K/year (enables sales)

  **Cost Savings**:
    - Reduces support costs (self-service)
    - Prevents security incidents
    - Estimated savings: $50K/year

  **Strategic Alignment**:
    - Aligns with security strategy
    - Supports user experience goals
    - Enables data collection and personalization

  **Competitive Advantage**:
    - Industry standard (expected feature)
    - Security is table stakes
    - No competitive advantage, but required to compete

  **ROI**: High - Required for business operations
```

### 8. Effort Estimation

**What to Document:**
- Development effort
- Testing effort
- Integration effort
- Total effort
- Resource requirements

**How to Find This:**
- Consult development team
- Review similar past projects
- Use estimation techniques (story points, hours)
- Consider complexity
- Account for dependencies

**Example:**
```markdown
**Effort Estimation for FR-045 (User Authentication)**:

  **Development Effort**:
    - Backend API: 2 weeks (1 developer)
    - Frontend UI: 1 week (1 developer)
    - Integration: 1 week (1 developer)
    - Security review: 3 days (security team)

  **Testing Effort**:
    - Unit tests: 3 days
    - Integration tests: 2 days
    - Security testing: 2 days
    - UAT: 2 days

  **Total Effort**: 4-5 weeks
  **Story Points**: 13 points (based on team velocity)
  **Resource Requirements**:
    - 2 backend developers
    - 1 frontend developer
    - 1 QA engineer
    - Security team (part-time)

  **Confidence Level**: High (80%) - Similar work done before
```

### 9. Timeline & Milestones

**What to Document:**
- Target release/phase
- Dependencies on timeline
- Critical dates
- Milestone alignment

**How to Find This:**
- Review project timeline
- Check release plans
- Consider dependencies
- Review milestone dates
- Align with business deadlines

**Example:**
```markdown
**Timeline for FR-045 (User Authentication)**:

  **Target Release**: MVP Release (Phase 1)
  **Target Date**: 2024-03-15
  **Dependencies**:
    - Must complete before FR-046 (User Profile)
    - Must complete before FR-047 (Access Control)
    - Blocks 15+ other requirements

  **Critical Dates**:
    - Start: 2024-02-01
    - Security review: 2024-02-20
    - Testing complete: 2024-03-05
    - Production deploy: 2024-03-15

  **Milestone Alignment**:
    - Part of MVP milestone
    - Required for beta launch
    - Critical path item

  **Flexibility**: Low - Cannot be delayed without impacting MVP
```

### 10. Decision & Rationale

**What to Document:**
- Final priority decision
- Priority category
- Rationale for decision
- Approvals
- Review date

**How to Find This:**
- Synthesize all analysis
- Make decision based on criteria
- Document reasoning
- Get stakeholder approval
- Set review schedule

**Example:**
```markdown
**Decision for FR-045 (User Authentication)**:

  **Final Priority**: Must Have (M) - Priority #1
  **Priority Category**: Critical

  **Rationale**:
    1. Critical for security and compliance
    2. Enables 15+ other requirements
    3. Required for MVP launch
    4. High business value (enables revenue)
    5. Low flexibility (cannot be delayed)
    6. High stakeholder consensus

  **Approvals**:
    - Product Owner: ✅ Approved
    - Technical Lead: ✅ Approved
    - Security Lead: ✅ Approved
    - Project Manager: ✅ Approved

  **Decision Date**: 2024-01-15
  **Next Review Date**: 2024-02-01 (if circumstances change)
  **Status**: Final - No changes expected
```

## Complete Example: E-Commerce Platform Requirements Prioritization

### Prioritization Document

```markdown
# Requirements Prioritization: E-Commerce Platform MVP

## Prioritization Method: Value vs. Effort Matrix + MoSCoW

**Date**: 2024-01-15
**Project**: E-Commerce Platform MVP
**Stakeholders**: Product Owner, Technical Lead, Business Analyst, UX Lead
**Total Requirements**: 45
**Prioritization Session**: 2024-01-10

---

## Requirement: FR-045 - User Authentication

### 1. Requirement Information

**Requirement ID**: FR-045
**Name**: User Authentication
**Type**: Functional Requirement
**Source**: Security Team, Product Owner
**Current Status**: Draft
**Related Requirements**:
  - NFR-002: Security Requirements
  - FR-046: User Profile Management
  - FR-047: Access Control

**Description**: 
System shall allow users to authenticate using email and password. System shall 
support password reset functionality and session management. Authentication must 
comply with security best practices including password hashing, rate limiting, 
and secure session tokens.

### 2. Prioritization Criteria

**Criteria Used**:
1. Business Value (30% weight)
2. User Impact (25% weight)
3. Technical Risk (20% weight)
4. Dependencies (15% weight)
5. Effort/Cost (10% weight)

**Scoring Scale**: 1-10 points per criterion

### 3. Stakeholder Input

**Stakeholders**:
- Product Owner: John Smith
- Technical Lead: Sarah Johnson
- Business Analyst: Mike Davis
- Security Lead: Lisa Chen
- UX Lead: Emily Brown

**Stakeholder Ratings** (1-10):

| Stakeholder | Business Value | User Impact | Tech Risk | Dependencies | Effort | Notes |
|------------|----------------|-------------|-----------|--------------|--------|-------|
| Product Owner | 10 | 9 | 7 | 10 | 6 | Critical for launch |
| Technical Lead | 9 | 8 | 8 | 10 | 7 | Foundation feature |
| Business Analyst | 9 | 9 | 7 | 9 | 6 | Core requirement |
| Security Lead | 10 | 8 | 6 | 10 | 8 | Security requirement |
| UX Lead | 8 | 10 | 8 | 9 | 5 | User experience critical |

**Average Scores**:
- Business Value: 9.2
- User Impact: 8.8
- Technical Risk: 7.2
- Dependencies: 9.6
- Effort: 6.4

**Consensus Level**: High - All stakeholders agree this is critical
**Conflicts**: None
**Discussion Notes**: 
- Security Lead emphasized importance of proper implementation
- Technical Lead noted this enables many other features
- Product Owner confirmed this is MVP requirement

### 4. Scoring & Ranking

**Weighted Scoring**:

| Criterion | Score | Weight | Weighted Score |
|-----------|-------|--------|----------------|
| Business Value | 9.2 | 30% | 2.76 |
| User Impact | 8.8 | 25% | 2.20 |
| Technical Risk | 7.2 | 20% | 1.44 |
| Dependencies | 9.6 | 15% | 1.44 |
| Effort/Cost | 6.4 | 10% | 0.64 |
| **Total** | | | **8.48 / 10.0** |

**Ranking**: #1 out of 45 requirements
**Priority Category**: Must Have (M)
**Value vs. Effort**: High Value, Medium Effort → Major Project

### 5. Dependencies & Relationships

**Depends On**:
- NFR-002: Security Requirements (encryption, TLS, etc.)
- FR-001: User Registration (users must register before login)
- NFR-010: Infrastructure (authentication service, database)
- FR-003: Email Service (for password reset)

**Enables** (15 requirements):
- FR-046: User Profile Management
- FR-047: Access Control
- FR-048: User Preferences
- FR-049: Order History
- FR-050: Wishlist
- FR-051: Saved Addresses
- FR-052: Payment Methods
- FR-053: Order Tracking
- FR-054: Returns Management
- FR-055: Reviews and Ratings
- FR-056: Recommendations
- FR-057: Loyalty Program
- FR-058: Notifications
- FR-059: Account Settings
- FR-060: Data Export

**Blocks**: None (foundational requirement)
**Critical Path**: Yes - Many features depend on this
**Impact of Delay**: High - Would delay 15+ requirements and MVP launch

### 6. Risk Assessment

**Technical Risks**:
- **Risk**: Integration with SSO providers (Google, Facebook) may be complex
- **Probability**: Medium
- **Impact**: Medium
- **Mitigation**: Use proven authentication library (Auth0), phase SSO for post-MVP

- **Risk**: Security vulnerabilities if not implemented correctly
- **Probability**: Low (with proper implementation)
- **Impact**: Critical
- **Mitigation**: Security review, penetration testing, use established libraries

**Business Risks**:
- **Risk**: Security breach if authentication is compromised
- **Probability**: Low
- **Impact**: Critical
- **Mitigation**: Security best practices, regular audits, monitoring

- **Risk**: User friction if authentication is too complex
- **Probability**: Medium
- **Impact**: Medium
- **Mitigation**: UX testing, clear error messages, password strength guidance

**Schedule Risks**:
- **Risk**: May delay other dependent features
- **Probability**: Medium
- **Impact**: High
- **Mitigation**: Prioritize early, allocate experienced developers, buffer time

**Resource Risks**:
- **Risk**: Security expertise may be limited
- **Probability**: Low
- **Impact**: Medium
- **Mitigation**: Use Auth0 (managed service), security team consultation

**Overall Risk Level**: Medium
**Risk Justification**: Manageable risks with proper planning and use of proven solutions

### 7. Business Value Analysis

**Business Value Score**: 10/10 (Critical)

**Revenue Impact**:
- Enables user accounts and personalized experience
- Required for e-commerce transactions (cart, checkout)
- Enables customer retention and repeat purchases
- Estimated revenue impact: $500K/year (enables all sales)
- Without this: Cannot launch MVP, $0 revenue

**Cost Savings**:
- Reduces support costs (self-service account management)
- Prevents security incidents (proper authentication)
- Reduces fraud (account verification)
- Estimated savings: $50K/year

**Strategic Alignment**:
- ✅ Aligns with security strategy (secure by design)
- ✅ Supports user experience goals (seamless authentication)
- ✅ Enables data collection and personalization
- ✅ Supports compliance (GDPR, PCI DSS requirements)

**Competitive Advantage**:
- Industry standard (expected feature)
- Security is table stakes (required to compete)
- No competitive advantage, but required to compete
- Differentiation comes from user experience, not authentication itself

**ROI**: 
- Investment: 4-5 weeks development + ongoing maintenance
- Return: Enables entire platform, $500K+ revenue/year
- ROI: Very High - Required for business operations

### 8. Effort Estimation

**Development Effort**:
- Backend API development: 2 weeks (1 developer)
  - Authentication endpoints
  - Password hashing and validation
  - Session management
  - Password reset flow
- Frontend UI development: 1 week (1 developer)
  - Login page
  - Registration page
  - Password reset UI
  - Error handling
- Integration: 1 week (1 developer)
  - Auth0 integration (if using)
  - Database integration
  - Email service integration
- Security review: 3 days (security team)
  - Code review
  - Penetration testing
  - Security audit

**Testing Effort**:
- Unit tests: 3 days (developer)
- Integration tests: 2 days (QA)
- Security testing: 2 days (security team)
- UAT: 2 days (stakeholders)

**Total Effort**: 4-5 weeks
**Story Points**: 13 points (based on team velocity of 20 points/sprint)
**Sprint Estimate**: 1.5 sprints (2-week sprints)

**Resource Requirements**:
- 2 backend developers (full-time)
- 1 frontend developer (full-time)
- 1 QA engineer (part-time, 50%)
- Security team (part-time, 20%)
- DevOps support (part-time, 10%)

**Confidence Level**: High (80%)
**Confidence Justification**: Similar authentication work done before, using proven library (Auth0)

**Assumptions**:
- Using Auth0 for authentication (reduces development time)
- Team has experience with authentication
- No custom SSO requirements for MVP
- Standard password requirements (no complex policies)

### 9. Timeline & Milestones

**Target Release**: MVP Release (Phase 1)
**Target Date**: 2024-03-15
**Phase**: MVP (Must Have)

**Dependencies Timeline**:
- Must complete before: FR-046 (User Profile) - starts 2024-03-16
- Must complete before: FR-047 (Access Control) - starts 2024-03-20
- Blocks: 15+ other requirements

**Critical Dates**:
- Start: 2024-02-01
- Backend complete: 2024-02-15
- Frontend complete: 2024-02-22
- Integration complete: 2024-03-01
- Security review: 2024-03-05
- Testing complete: 2024-03-10
- Production deploy: 2024-03-15

**Milestone Alignment**:
- ✅ Part of MVP milestone
- ✅ Required for beta launch (2024-03-20)
- ✅ Critical path item
- ✅ Blocks user-facing features

**Flexibility**: Low
**Flexibility Justification**: Cannot be delayed without impacting MVP launch date and 15+ dependent requirements

**Contingency Plan**: 
- If delayed, consider using Auth0 managed service to accelerate
- May need to reduce scope (remove SSO for MVP, add post-MVP)

### 10. Decision & Rationale

**Final Priority**: Must Have (M) - Priority #1
**Priority Category**: Critical
**Value vs. Effort**: High Value, Medium Effort → Major Project (do it, plan carefully)

**Decision Rationale**:
1. **Critical for Security**: Required for secure user accounts and data protection
2. **Enables Many Features**: Blocks 15+ other requirements, foundational feature
3. **Required for MVP**: Cannot launch without user authentication
4. **High Business Value**: Enables entire platform and revenue generation
5. **Low Flexibility**: Cannot be delayed without major impact
6. **High Stakeholder Consensus**: All stakeholders agree this is critical
7. **Manageable Risk**: Risks are manageable with proper planning
8. **Reasonable Effort**: 4-5 weeks is acceptable for critical feature

**Alternative Considered**: 
- Use third-party authentication only (Auth0) - **Rejected**: Still need custom implementation for MVP features
- Delay to post-MVP - **Rejected**: Blocks too many requirements

**Approvals**:
- Product Owner: ✅ Approved (2024-01-10)
- Technical Lead: ✅ Approved (2024-01-10)
- Security Lead: ✅ Approved (2024-01-10)
- Project Manager: ✅ Approved (2024-01-10)
- Business Analyst: ✅ Approved (2024-01-10)

**Decision Date**: 2024-01-15
**Decision Maker**: Product Owner (with stakeholder consensus)
**Next Review Date**: 2024-02-01 (if circumstances change)
**Status**: Final - Approved for MVP Phase 1

**Notes**: 
- This is the highest priority requirement
- Must start immediately (2024-02-01)
- Allocate best developers to ensure quality and timeline
- Security review is mandatory before production deployment
```

## How to Find Details for Each Element

### Finding Requirement Information

**Sources:**
1. **Requirements Documents**: Review existing requirements
   - Check [Functional Requirements](./Functional%20Requirements.md)
   - Check [Non-Functional Requirements](./Non-Functional%20Requirements.md)
   - Review [Business Requirements](./Business%20Requirements.md)
   - Check [User Requirements](./User%20Requirements.md)
   - Review [System Requirements](./System%20Requirements.md)

2. **Requirements Management Tools**: Extract from tools
   - Jira, Azure DevOps, ReqView
   - Requirements databases
   - Spreadsheets

3. **Stakeholder Documents**: Review stakeholder input
   - Interview notes
   - Workshop outputs
   - User stories

**Tools:**
- **Requirements Management**: Jira, Azure DevOps, ReqView
- **Documentation**: Confluence, Notion
- **Spreadsheets**: Excel, Google Sheets

**Practical Method:**
```bash
# Search requirements documents
grep -r "FR-\|NFR-\|REQ-" docs/
# Extract requirement IDs and names
# Compile into prioritization list
```

### Finding Prioritization Criteria

**Sources:**
1. **Business Objectives**: Review project goals
   - Check [Project Charter](./Project%20Charter.md)
   - Review [Business Requirements](./Business%20Requirements.md)
   - Analyze business strategy
   - Consider ROI objectives

2. **Stakeholder Input**: Get criteria from stakeholders
   - Conduct workshops
   - Survey stakeholders
   - Review interview notes
   - Hold prioritization sessions

3. **Industry Best Practices**: Research methods
   - MoSCoW method
   - Value vs. Effort matrix
   - RICE scoring
   - WSJF (SAFe)

4. **Project Constraints**: Consider limitations
   - Budget constraints
   - Timeline constraints
   - Resource constraints
   - Technical constraints

**Tools:**
- **Workshops**: Miro, Mural, whiteboards
- **Surveys**: SurveyMonkey, Google Forms
- **Research**: Industry articles, case studies

**Practical Method:**
```markdown
1. Review business objectives
2. Conduct stakeholder workshop
3. List potential criteria
4. Vote on most important criteria
5. Assign weights based on importance
6. Define scoring scales
```

### Finding Stakeholder Input

**Sources:**
1. **Stakeholder Interviews**: Review interviews
   - Check [Structured Interviews](./Structured%20Interviews.md)
   - Check [Unstructured Interviews](./Unstructured%20Interviews.md)
   - Review interview transcripts
   - Extract priorities

2. **Prioritization Workshops**: Conduct sessions
   - Planning poker
   - Dot voting
   - Value vs. Effort voting
   - Consensus building

3. **Surveys**: Collect input
   - Online surveys
   - Rating scales
   - Ranking exercises

4. **Meetings**: Regular prioritization
   - Sprint planning
   - Release planning
   - Backlog refinement

**Tools:**
- **Workshops**: Miro, Mural, FigJam
- **Voting**: Planning poker apps, dot voting tools
- **Surveys**: SurveyMonkey, Google Forms, Typeform
- **Collaboration**: Slack, Microsoft Teams

**Practical Method:**
```markdown
1. Identify key stakeholders
2. Schedule prioritization workshop
3. Use voting technique (dot voting, planning poker)
4. Collect ratings/rankings
5. Analyze consensus and conflicts
6. Document input
```

### Finding Scoring & Ranking

**Sources:**
1. **Calculation**: Compute scores
   - Apply criteria weights
   - Calculate weighted scores
   - Sum total scores
   - Rank by score

2. **Tools**: Use prioritization tools
   - Jira prioritization
   - Product management tools
   - Custom spreadsheets
   - Prioritization apps

**Tools:**
- **Spreadsheets**: Excel, Google Sheets (formulas)
- **Jira**: Priority fields, custom fields
- **Product Tools**: Productboard, Aha!, Roadmunk
- **Custom Tools**: Build prioritization calculator

**Practical Method:**
```markdown
1. Create scoring spreadsheet
2. Enter criteria and weights
3. Enter stakeholder ratings
4. Calculate weighted scores
5. Sort by total score
6. Assign priority categories
```

### Finding Dependencies & Relationships

**Sources:**
1. **Requirements Traceability**: Map relationships
   - Review requirement dependencies
   - Check traceability matrix
   - Analyze functional dependencies
   - Review technical dependencies

2. **Architecture Analysis**: Understand system structure
   - Review architecture documents
   - Check system design
   - Understand component dependencies
   - Review data flows

3. **Team Input**: Consult technical team
   - Development team knowledge
   - Architecture team input
   - Dependency analysis

**Tools:**
- **Requirements Management**: Jira (links), Azure DevOps (dependencies)
- **Diagramming**: Draw.io, Lucidchart (dependency diagrams)
- **Analysis**: Dependency matrices, graphs

**Practical Method:**
```markdown
1. Review requirements for "depends on" statements
2. Consult technical team
3. Create dependency diagram
4. Identify critical path
5. Document blocking relationships
```

### Finding Risk Assessment

**Sources:**
1. **Risk Registers**: Review existing risks
   - Project risk register
   - Technical risk analysis
   - Business risk assessment

2. **Team Analysis**: Consult experts
   - Technical team (technical risks)
   - Business team (business risks)
   - Security team (security risks)
   - QA team (quality risks)

3. **Historical Data**: Learn from past
   - Similar past projects
   - Team experience
   - Industry data

**Tools:**
- **Risk Management**: Risk registers, risk matrices
- **Analysis**: Risk assessment templates
- **Tracking**: Risk tracking tools

**Practical Method:**
```markdown
1. Review requirement for risks
2. Consult relevant experts
3. Assess probability and impact
4. Document mitigation strategies
5. Calculate overall risk level
```

### Finding Business Value Analysis

**Sources:**
1. **Business Requirements**: Review business needs
   - Check [Business Requirements](./Business%20Requirements.md)
   - Review [Project Charter](./Project%20Charter.md)
   - Analyze business objectives

2. **Financial Analysis**: Estimate impact
   - Revenue impact
   - Cost savings
   - ROI calculation
   - Financial modeling

3. **Stakeholder Input**: Get business perspective
   - Business stakeholders
   - Product owners
   - Executive input

**Tools:**
- **Financial Analysis**: Spreadsheets, financial models
- **Business Analysis**: Business case templates
- **ROI Calculators**: Custom calculators

**Practical Method:**
```markdown
1. Review business objectives
2. Estimate revenue impact
3. Estimate cost savings
4. Calculate ROI
5. Assess strategic alignment
6. Document business value
```

### Finding Effort Estimation

**Sources:**
1. **Development Team**: Get estimates
   - Story point estimation
   - Time estimation
   - Team velocity data
   - Historical data

2. **Estimation Techniques**: Use methods
   - Planning poker
   - T-shirt sizing
   - Three-point estimation
   - Analogous estimation

3. **Similar Projects**: Learn from past
   - Similar requirements
   - Team experience
   - Historical data

**Tools:**
- **Estimation**: Planning poker apps, estimation tools
- **Tracking**: Jira, Azure DevOps (story points, time tracking)
- **Velocity**: Team velocity charts, burndown charts

**Practical Method:**
```markdown
1. Break requirement into tasks
2. Use planning poker or similar
3. Get team estimates
4. Consider complexity and risk
5. Add buffer for uncertainty
6. Document assumptions
```

### Finding Timeline & Milestones

**Sources:**
1. **Project Plan**: Review timeline
   - Project schedule
   - Release plan
   - Milestone dates
   - Phase planning

2. **Dependencies**: Consider dependencies
   - Requirement dependencies
   - Resource dependencies
   - External dependencies

3. **Business Deadlines**: Consider constraints
   - Launch dates
   - Business deadlines
   - Regulatory deadlines
   - Market windows

**Tools:**
- **Project Management**: Jira, Azure DevOps, MS Project
- **Timeline**: Gantt charts, timeline tools
- **Planning**: Release planning tools

**Practical Method:**
```markdown
1. Review project timeline
2. Consider dependencies
3. Check business deadlines
4. Align with milestones
5. Document critical dates
```

### Finding Decision & Rationale

**Sources:**
1. **Synthesis**: Combine all analysis
   - Review all elements
   - Synthesize information
   - Make informed decision
   - Document rationale

2. **Stakeholder Approval**: Get buy-in
   - Present analysis
   - Get approvals
   - Document decisions
   - Set review schedule

**Tools:**
- **Documentation**: Decision logs, meeting notes
- **Approval**: Approval workflows, sign-offs
- **Tracking**: Decision tracking tools

**Practical Method:**
```markdown
1. Review all analysis
2. Make priority decision
3. Document rationale
4. Get stakeholder approval
5. Set review date
6. Communicate decision
```

## Practical Tools for Requirements Prioritization

### Prioritization Tools

**Dedicated Prioritization Tools:**
- **Productboard**: Product management with prioritization
- **Aha!**: Roadmapping and prioritization
- **Roadmunk**: Roadmap and prioritization
- **Reqqo**: Requirements prioritization

**General Tools:**
- **Jira**: Issue prioritization with custom fields
- **Azure DevOps**: Backlog prioritization
- **Trello**: Card prioritization
- **Asana**: Task prioritization

### Workshop & Collaboration Tools

**Virtual Whiteboards:**
- **Miro**: Collaborative whiteboard
- **Mural**: Digital workspace
- **Figma**: Design and collaboration
- **Miroverse**: Prioritization templates

**Voting Tools:**
- **Planning Poker**: Story point estimation
- **Dot Voting**: Simple prioritization
- **Priority Matrix**: Value vs. Effort
- **Custom Voting Apps**: Build your own

### Analysis & Calculation Tools

**Spreadsheets:**
- **Excel**: Formulas and calculations
- **Google Sheets**: Collaborative analysis
- **Airtable**: Database-like spreadsheets

**Custom Calculators:**
- **RICE Calculator**: Online RICE scoring
- **WSJF Calculator**: SAFe WSJF calculation
- **Priority Matrix**: Value vs. Effort plotting

### Visualization Tools

**Charts & Graphs:**
- **Excel/Google Sheets**: Charts and graphs
- **Tableau**: Data visualization
- **Power BI**: Business intelligence
- **Custom Dashboards**: Build prioritization dashboards

**Matrices:**
- **Value vs. Effort Matrix**: 2x2 matrix
- **Priority Matrix**: Multi-criteria matrix
- **Dependency Graph**: Requirement dependencies

## Practical Workflow: Step-by-Step

### Step 1: Prepare Requirements List

**Activities:**
1. Collect all requirements
2. Organize by type
3. Assign unique IDs
4. Create prioritization spreadsheet
5. Prepare requirement summaries

**Output:** Prioritization-ready requirements list

**Time:** 2-4 hours

**Tools:**
- Requirements documents
- Requirements management tools
- Spreadsheets

### Step 2: Define Prioritization Method

**Activities:**
1. Choose prioritization method(s)
2. Define criteria
3. Assign weights
4. Set scoring scales
5. Document method

**Output:** Prioritization method and criteria

**Time:** 2-4 hours

**Tools:**
- Method selection
- Criteria definition
- Weight assignment

### Step 3: Gather Stakeholder Input

**Activities:**
1. Identify stakeholders
2. Schedule workshop
3. Conduct prioritization session
4. Collect ratings/rankings
5. Document input

**Output:** Stakeholder input and ratings

**Time:** 4-8 hours (workshop + follow-up)

**Tools:**
- Workshop tools
- Voting tools
- Collaboration platforms

### Step 4: Analyze & Score

**Activities:**
1. Calculate scores
2. Apply weights
3. Rank requirements
4. Identify conflicts
5. Analyze patterns

**Output:** Scored and ranked requirements

**Time:** 4-8 hours

**Tools:**
- Spreadsheets
- Calculation tools
- Analysis tools

### Step 5: Document Dependencies

**Activities:**
1. Map requirement dependencies
2. Identify critical path
3. Document blocking relationships
4. Analyze impact
5. Create dependency diagram

**Output:** Dependency map and analysis

**Time:** 2-4 hours

**Tools:**
- Dependency mapping
- Diagramming tools
- Analysis tools

### Step 6: Assess Risks & Value

**Activities:**
1. Assess risks for each requirement
2. Analyze business value
3. Estimate effort
4. Consider timeline
5. Document analysis

**Output:** Risk and value analysis

**Time:** 4-8 hours

**Tools:**
- Risk assessment
- Business analysis
- Estimation tools

### Step 7: Make Decisions

**Activities:**
1. Synthesize all analysis
2. Make priority decisions
3. Assign priority categories
4. Document rationale
5. Get approvals

**Output:** Prioritized requirements with decisions

**Time:** 2-4 hours

**Tools:**
- Decision documentation
- Approval workflows
- Communication tools

### Step 8: Communicate & Review

**Activities:**
1. Communicate priorities
2. Update requirements
3. Update project plan
4. Set review schedule
5. Monitor and adjust

**Output:** Communicated priorities and review plan

**Time:** 2-4 hours

**Tools:**
- Communication tools
- Project management tools
- Documentation tools

**Total Time:** 22-44 hours (typically 3-5 days)

## Best Practices

### Do's

✅ **Involve Key Stakeholders**
- Get diverse perspectives
- Ensure buy-in
- Balance competing needs
- Build consensus

✅ **Use Multiple Methods**
- Combine methods for better results
- Use appropriate method for context
- Validate with different approaches
- Consider multiple factors

✅ **Make Criteria Explicit**
- Define clear criteria
- Assign weights
- Use consistent scales
- Document rationale

✅ **Document Thoroughly**
- Document all elements
- Record decisions and rationale
- Track changes
- Maintain traceability

✅ **Review Regularly**
- Re-prioritize as needed
- Respond to changes
- Update based on feedback
- Monitor and adjust

### Don'ts

❌ **Don't Prioritize in Isolation**
- Involve stakeholders
- Consider multiple perspectives
- Don't ignore dependencies
- Don't skip analysis

❌ **Don't Use Only One Method**
- Combine methods
- Validate with different approaches
- Consider context
- Don't rely on single metric

❌ **Don't Ignore Dependencies**
- Map dependencies
- Consider critical path
- Account for blocking relationships
- Plan accordingly

❌ **Don't Set and Forget**
- Review regularly
- Respond to changes
- Update priorities
- Monitor and adjust

❌ **Don't Skip Documentation**
- Document decisions
- Record rationale
- Maintain traceability
- Track changes

## Common Pitfalls & How to Avoid Them

### Pitfall 1: Too Many "Must Haves"

**Problem:** Everything becomes critical, no real prioritization

**Solution:**
- Use strict criteria for "Must Have"
- Limit percentage (e.g., max 20% Must Have)
- Force trade-offs
- Use value vs. effort matrix

### Pitfall 2: Ignoring Dependencies

**Problem:** Prioritizing without considering dependencies

**Solution:**
- Map all dependencies
- Identify critical path
- Consider blocking relationships
- Plan accordingly

### Pitfall 3: Subjective Prioritization

**Problem:** Prioritization based on opinions, not data

**Solution:**
- Use objective criteria
- Collect data
- Use multiple methods
- Document rationale

### Pitfall 4: Not Involving Stakeholders

**Problem:** Prioritization done in isolation

**Solution:**
- Involve key stakeholders
- Get diverse perspectives
- Build consensus
- Ensure buy-in

### Pitfall 5: Not Reviewing Regularly

**Problem:** Priorities set once and never updated

**Solution:**
- Schedule regular reviews
- Respond to changes
- Update based on feedback
- Monitor and adjust

## Integration with Requirements Process

Requirements Prioritization is part of the complete requirements process:

1. **Requirements Elicitation**: Gather requirements
2. **Requirements Analysis**: Analyze requirements
3. **Requirements Categorization**: Categorize requirements
4. **Requirements Prioritization**: Prioritize requirements ← **You are here**
5. **Requirements Validation**: Validate requirements
6. **Requirements Management**: Manage requirements

See [Planning & Requirements Gathering](./Planning%20&%20Requirements%20Gathering.md) for the complete requirements process.

## Relationship with Other Requirements Activities

**Requirements Categorization**: Groups requirements by type
**Requirements Prioritization**: Ranks requirements by importance

**Example:**
- **Categorization**: Functional, Non-Functional, Business, User, System
- **Prioritization**: Must Have, Should Have, Could Have, Won't Have

Both are essential for effective requirements management.

## Conclusion

Requirements Prioritization is critical for:
- **Focusing efforts** on high-value requirements
- **Managing resources** effectively
- **Delivering value** early
- **Managing risk** by addressing critical items first
- **Balancing** competing stakeholder needs

Key success factors:
- ✅ Involve key stakeholders
- ✅ Use appropriate methods
- ✅ Make criteria explicit
- ✅ Document thoroughly
- ✅ Review regularly
- ✅ Consider dependencies
- ✅ Balance multiple factors

Remember: Prioritization is not a one-time activity. It's an ongoing process that requires regular review and adjustment as requirements, constraints, and business needs evolve. Effective prioritization ensures that development efforts focus on delivering the most value to stakeholders.

