---
title: "Requirements Modeling - Detailed Guide"
description: "Comprehensive guide to Requirements Modeling: Visual representation of requirements using diagrams and models"
author: "Development Team"
date: "2024"
---

# Requirements Modeling: Visual Representation of Requirements

## Overview

**Requirements Modeling** is the process of creating visual representations of requirements using diagrams, models, and graphical notations. It helps stakeholders understand requirements better, identifies gaps and inconsistencies, facilitates communication, and supports system design and development.

## Definition

Requirements Modeling is:
- **Visual representation** of requirements using diagrams
- **Communication tool** for stakeholders
- **Analysis technique** for requirement validation
- **Design foundation** for system architecture
- **Documentation method** for requirements specification

## Key Characteristics

### Visual
- Uses diagrams and models
- Graphical representation
- Easy to understand
- Communicates complex ideas

### Standardized
- Uses standard notations (UML, BPMN, etc.)
- Consistent symbols and conventions
- Industry-recognized standards
- Tool-supported

### Comprehensive
- Covers multiple perspectives
- Shows relationships
- Identifies gaps
- Validates completeness

### Traceable
- Links to requirements
- Maintains relationships
- Supports analysis
- Enables validation

## Benefits of Requirements Modeling

### Improved Understanding
- Visual representation is easier to understand
- Clarifies complex requirements
- Identifies relationships
- Shows system behavior

### Better Communication
- Common language for stakeholders
- Reduces misunderstandings
- Facilitates discussions
- Supports presentations

### Gap Identification
- Reveals missing requirements
- Identifies inconsistencies
- Shows incomplete flows
- Highlights edge cases

### Design Foundation
- Guides system design
- Informs architecture
- Supports implementation
- Enables testing

## Types of Requirements Models

### 1. Use Case Diagrams

**Definition**: Shows interactions between actors (users, systems) and the system to achieve goals.

**Purpose**: 
- Identify system functionality
- Show user interactions
- Define system boundaries
- Document user goals

**Best For**: 
- Functional requirements
- User interactions
- System scope definition
- Requirements validation

**Elements**:
- Actors (users, external systems)
- Use cases (system functions)
- System boundary
- Relationships (associations, includes, extends, generalizes)

### 2. Activity Diagrams

**Definition**: Shows workflows, business processes, and system activities with decision points and parallel flows.

**Purpose**:
- Model business processes
- Show workflow steps
- Identify decision points
- Document parallel activities

**Best For**:
- Business process modeling
- Workflow documentation
- Process analysis
- Requirements validation

**Elements**:
- Activities (actions)
- Decisions (diamonds)
- Forks/Joins (parallel flows)
- Start/End nodes
- Swimlanes (actors/responsibilities)

### 3. Data Flow Diagrams (DFD)

**Definition**: Shows how data flows through a system, including processes, data stores, and external entities.

**Purpose**:
- Model data flow
- Identify data transformations
- Show data stores
- Document data requirements

**Best For**:
- Data requirements
- System analysis
- Data flow understanding
- Integration requirements

**Elements**:
- Processes (circles/rounded rectangles)
- Data stores (open rectangles)
- External entities (rectangles)
- Data flows (arrows with labels)

### 4. Entity Relationship Diagrams (ERD)

**Definition**: Shows data structure, entities, attributes, and relationships in a system.

**Purpose**:
- Model data structure
- Define entities and attributes
- Show relationships
- Document data requirements

**Best For**:
- Database design
- Data modeling
- Data requirements
- System design

**Elements**:
- Entities (rectangles)
- Attributes (ovals or listed)
- Relationships (diamonds or lines)
- Cardinality (one-to-one, one-to-many, many-to-many)

### 5. State Diagrams (State Machines)

**Definition**: Shows how system or objects change states in response to events.

**Purpose**:
- Model state changes
- Show state transitions
- Identify events and triggers
- Document behavior requirements

**Best For**:
- State-based systems
- Workflow states
- Object lifecycle
- Behavior requirements

**Elements**:
- States (rounded rectangles)
- Transitions (arrows)
- Events/Triggers (labels on arrows)
- Initial state (filled circle)
- Final state (circle with X)

### 6. Sequence Diagrams

**Definition**: Shows interactions between objects/components over time, showing message exchanges.

**Purpose**:
- Model interactions
- Show message flow
- Identify timing
- Document communication requirements

**Best For**:
- Interaction modeling
- API design
- Component communication
- Integration requirements

**Elements**:
- Lifelines (objects/components)
- Messages (arrows)
- Activation boxes (execution)
- Time flow (top to bottom)

### 7. Class Diagrams

**Definition**: Shows system structure with classes, attributes, methods, and relationships.

**Purpose**:
- Model system structure
- Define classes and objects
- Show relationships
- Document structural requirements

**Best For**:
- Object-oriented design
- System structure
- Data modeling
- Architecture design

**Elements**:
- Classes (rectangles with compartments)
- Attributes
- Methods/Operations
- Relationships (association, inheritance, composition)

### 8. Business Process Model and Notation (BPMN)

**Definition**: Standard notation for modeling business processes with events, activities, gateways, and flows.

**Purpose**:
- Model business processes
- Standard notation
- Process documentation
- Requirements analysis

**Best For**:
- Business process modeling
- Workflow documentation
- Process automation
- Business requirements

**Elements**:
- Events (start, intermediate, end)
- Activities (tasks, sub-processes)
- Gateways (decisions, parallel)
- Flows (sequence, message)
- Swimlanes (pools, lanes)

## Essential Elements of Requirements Modeling

### 1. Model Purpose & Scope

**What to Document:**
- Purpose of the model
- Scope and boundaries
- Level of detail
- Target audience
- Related requirements

**How to Find This:**
- Review requirements documents
- Check [Functional Requirements](./Functional%20Requirements.md)
- Review [Business Requirements](./Business%20Requirements.md)
- Understand modeling objectives
- Identify stakeholders

**Example:**
```markdown
**Model Purpose**: 
Create use case diagram for user authentication system to visualize all 
authentication-related functionality and identify actors and use cases.

**Scope**: 
- User authentication (login, logout, password reset)
- User registration
- Session management
- Excludes: Authorization, user profile management

**Level of Detail**: High-level (system use cases, not detailed steps)
**Target Audience**: Product Owner, Development Team, QA Team
**Related Requirements**: FR-045 (User Authentication), FR-046 (User Registration)
```

### 2. Model Type & Notation

**What to Document:**
- Type of model (Use Case, Activity, etc.)
- Notation standard (UML, BPMN, etc.)
- Version of standard
- Tool used
- Conventions used

**How to Find This:**
- Select appropriate model type
- Choose standard notation
- Select modeling tool
- Define conventions
- Document standards

**Example:**
```markdown
**Model Type**: Use Case Diagram
**Notation Standard**: UML 2.5
**Tool**: Lucidchart
**Conventions**:
  - Actors: Stick figures
  - Use cases: Ovals
  - System boundary: Rectangle
  - Relationships: Solid lines (association), dashed lines (include/extend)
  - <<include>>: Mandatory relationship
  - <<extend>>: Optional relationship

**Version**: 1.0
**Last Updated**: 2024-01-15
```

### 3. Model Elements

**What to Document:**
- All elements in the model
- Element names and descriptions
- Relationships between elements
- Properties and attributes
- Constraints and rules

**How to Find This:**
- Extract from requirements
- Identify from stakeholder discussions
- Review [Structured Interviews](./Structured%20Interviews.md)
- Review [Unstructured Interviews](./Unstructured%20Interviews.md)
- Analyze business processes

**Example:**
```markdown
**Actors**:
  1. **Registered User**
     - Description: User who has created an account
     - Interactions: Login, logout, password reset
     - Related Requirements: FR-045

  2. **New User**
     - Description: User who wants to create an account
     - Interactions: Register, verify email
     - Related Requirements: FR-046

  3. **System Administrator**
     - Description: Admin managing user accounts
     - Interactions: View users, manage accounts
     - Related Requirements: FR-047

**Use Cases**:
  1. **Login**
     - Description: User authenticates with email and password
     - Actors: Registered User
     - Includes: Validate credentials
     - Related Requirements: FR-045-001

  2. **Logout**
     - Description: User ends session
     - Actors: Registered User
     - Related Requirements: FR-045-002

  3. **Register**
     - Description: New user creates account
     - Actors: New User
     - Includes: Validate email, create account
     - Related Requirements: FR-046-001

  4. **Reset Password**
     - Description: User resets forgotten password
     - Actors: Registered User
     - Extends: Login (if user forgot password)
     - Related Requirements: FR-045-003
```

### 4. Relationships & Dependencies

**What to Document:**
- Relationships between elements
- Dependencies
- Includes and extends relationships
- Generalization relationships
- Association relationships

**How to Find This:**
- Analyze element relationships
- Review requirement dependencies
- Check [Requirements Prioritization](./Requirements%20Prioritization.md)
- Understand functional dependencies
- Map relationships

**Example:**
```markdown
**Relationships**:

  1. **Login <<includes>> Validate Credentials**
     - Type: Include (mandatory)
     - Description: Login always includes credential validation
     - Related Requirements: FR-045-001

  2. **Login <<extends>> Reset Password**
     - Type: Extend (optional)
     - Description: User can reset password if they forgot it during login
     - Condition: User clicks "Forgot Password" link
     - Related Requirements: FR-045-003

  3. **Register <<includes>> Validate Email**
     - Type: Include (mandatory)
     - Description: Registration always validates email format
     - Related Requirements: FR-046-002

  4. **Register <<includes>> Create Account**
     - Type: Include (mandatory)
     - Description: Registration creates user account
     - Related Requirements: FR-046-001

**Dependencies**:
  - Register must complete before Login (user must have account)
  - Reset Password requires valid email (from registration)
  - All use cases depend on authentication infrastructure
```

### 5. Business Rules & Constraints

**What to Document:**
- Business rules
- Constraints
- Validation rules
- Preconditions
- Postconditions

**How to Find This:**
- Review [Business Requirements](./Business%20Requirements.md)
- Check [Business Process Document](./Business%20Process%20Document.md)
- Review stakeholder discussions
- Analyze business logic
- Document constraints

**Example:**
```markdown
**Business Rules**:

  1. **Email Validation**
     - Rule: Email must be valid format and unique
     - Applies to: Register, Reset Password
     - Related Requirements: FR-046-002

  2. **Password Requirements**
     - Rule: Password must be 8+ characters, include uppercase, lowercase, number
     - Applies to: Register, Reset Password
     - Related Requirements: NFR-002 (Security)

  3. **Session Timeout**
     - Rule: Session expires after 30 minutes of inactivity
     - Applies to: Login, all authenticated sessions
     - Related Requirements: FR-045-004

  4. **Account Lockout**
     - Rule: Account locked after 5 failed login attempts
     - Applies to: Login
     - Related Requirements: NFR-002 (Security)

**Constraints**:
  - Must support email and password only (no SSO for MVP)
  - Must comply with GDPR (data protection)
  - Must use HTTPS (security requirement)
  - Must support password reset via email only
```

### 6. Model Validation

**What to Document:**
- Validation criteria
- Completeness check
- Consistency check
- Stakeholder review
- Approval status

**How to Find This:**
- Define validation criteria
- Review with stakeholders
- Check for completeness
- Verify consistency
- Get approvals

**Example:**
```markdown
**Validation Criteria**:

  1. **Completeness**
     - ✅ All actors identified
     - ✅ All use cases documented
     - ✅ All relationships shown
     - ✅ System boundary defined

  2. **Consistency**
     - ✅ Use case names match requirements
     - ✅ Actor names consistent
     - ✅ Relationships logical
     - ✅ No contradictions

  3. **Traceability**
     - ✅ All use cases linked to requirements
     - ✅ All actors linked to user requirements
     - ✅ Relationships documented

**Stakeholder Review**:
  - Product Owner: ✅ Approved (2024-01-15)
  - Development Team: ✅ Approved (2024-01-15)
  - QA Team: ✅ Approved (2024-01-16)
  - Security Team: ✅ Approved (2024-01-16)

**Validation Status**: ✅ Validated and Approved
**Issues Found**: None
**Changes Made**: None
```

### 7. Model Maintenance

**What to Document:**
- Version history
- Change log
- Update schedule
- Owner/responsible person
- Review dates

**How to Find This:**
- Track model versions
- Document changes
- Set review schedule
- Assign ownership
- Plan updates

**Example:**
```markdown
**Version History**:
  - v1.0 (2024-01-15): Initial version
  - v1.1 (2024-01-20): Added "Remember Me" use case
  - v1.2 (2024-02-01): Added System Administrator actor

**Change Log**:
  - 2024-01-20: Added "Remember Me" use case (extend Login)
  - 2024-02-01: Added System Administrator actor and related use cases
  - 2024-02-15: Updated relationships based on new requirements

**Update Schedule**: Review monthly or when requirements change
**Owner**: Business Analyst (Sarah Johnson)
**Last Review**: 2024-02-15
**Next Review**: 2024-03-15
```

### 8. Tool & Format Information

**What to Document:**
- Modeling tool used
- File format
- Export formats
- Access information
- Tool version

**How to Find This:**
- Select modeling tool
- Document tool details
- Specify file formats
- Provide access info
- Note tool version

**Example:**
```markdown
**Modeling Tool**: Lucidchart
**Tool Version**: Latest (2024)
**File Format**: .lucid (Lucidchart native)
**Export Formats**: 
  - PDF (for documentation)
  - PNG (for presentations)
  - SVG (for web)
  - Visio (for compatibility)

**File Location**: 
  - Cloud: Lucidchart workspace "E-Commerce Project"
  - Local: docs/models/use-case-authentication.lucid
  - Documentation: docs/models/use-case-authentication.pdf

**Access**: 
  - Team members: Full access
  - Stakeholders: View-only access
  - Public: Not shared
```

## Complete Example: E-Commerce Platform Use Case Model

### Use Case Diagram Example

```markdown
# Use Case Model: E-Commerce Platform - User Management

## 1. Model Purpose & Scope

**Model Purpose**: 
Create comprehensive use case diagram for user management functionality in 
e-commerce platform, including authentication, registration, and profile management.

**Scope**: 
- User authentication (login, logout, password management)
- User registration and account creation
- User profile management
- Account settings
- Excludes: Order management, payment processing, product browsing

**Level of Detail**: System-level use cases (not detailed steps)
**Target Audience**: Product Owner, Development Team, QA Team, UX Team
**Related Requirements**: 
  - FR-045: User Authentication
  - FR-046: User Registration
  - FR-047: User Profile Management
  - FR-048: Account Settings

**Model Date**: 2024-01-15
**Version**: 1.0

## 2. Model Type & Notation

**Model Type**: Use Case Diagram
**Notation Standard**: UML 2.5
**Tool**: Lucidchart
**Conventions**:
  - Actors: Stick figures with role names
  - Use cases: Ovals with use case names
  - System boundary: Rectangle labeled "E-Commerce Platform"
  - Associations: Solid lines (actor to use case)
  - <<include>>: Dashed arrow with <<include>> stereotype (mandatory)
  - <<extend>>: Dashed arrow with <<extend>> stereotype (optional)
  - Generalization: Solid line with arrow (inheritance)

**Diagram Style**:
  - Actors outside system boundary
  - Use cases inside system boundary
  - Grouped by functional area
  - Color-coded by priority (red: Must Have, yellow: Should Have, green: Could Have)

## 3. Model Elements

### Actors

**1. Customer**
   - **Description**: End user shopping on the platform
   - **Characteristics**: 
     - May be registered or guest
     - Primary user of the system
     - Can browse, search, and purchase
   - **Interactions**: 
     - Register account
     - Login/Logout
     - Manage profile
     - Update account settings
   - **Related Requirements**: FR-045, FR-046, FR-047, FR-048
   - **Priority**: Critical

**2. Guest User**
   - **Description**: Unregistered user browsing the platform
   - **Characteristics**:
     - Not authenticated
     - Limited functionality
     - Can register to become Customer
   - **Interactions**:
     - Register account
     - Browse products (not in this model)
   - **Related Requirements**: FR-046
   - **Priority**: Critical
   - **Note**: Generalizes to Customer after registration

**3. System Administrator**
   - **Description**: Admin managing user accounts and system
   - **Characteristics**:
     - Full system access
     - Manages user accounts
     - Monitors system
   - **Interactions**:
     - View all users
     - Manage user accounts
     - Reset user passwords
     - Deactivate accounts
   - **Related Requirements**: FR-049 (Admin Functions)
   - **Priority**: High

**4. Email System**
   - **Description**: External system for sending emails
   - **Characteristics**:
     - External system
     - Automated email sending
   - **Interactions**:
     - Send registration confirmation
     - Send password reset email
     - Send account updates
   - **Related Requirements**: FR-046, FR-045-003
   - **Priority**: Critical

### Use Cases

**Authentication Use Cases:**

**UC-001: Login**
   - **Description**: Customer authenticates with email and password
   - **Actors**: Customer
   - **Priority**: Must Have (M)
   - **Includes**: 
     - Validate Credentials
     - Create Session
   - **Extends**: 
     - Reset Password (if forgot password)
   - **Preconditions**: 
     - Customer has registered account
     - Customer has valid email and password
   - **Postconditions**: 
     - Customer is authenticated
     - Session is created
   - **Related Requirements**: FR-045-001
   - **Business Rules**:
     - Maximum 5 failed attempts before account lockout
     - Session timeout: 30 minutes inactivity

**UC-002: Logout**
   - **Description**: Customer ends their session
   - **Actors**: Customer
   - **Priority**: Must Have (M)
   - **Preconditions**: 
     - Customer is logged in
   - **Postconditions**: 
     - Session is terminated
     - Customer is logged out
   - **Related Requirements**: FR-045-002

**UC-003: Reset Password**
   - **Description**: Customer resets forgotten password via email
   - **Actors**: Customer, Email System
   - **Priority**: Must Have (M)
   - **Extends**: Login (optional extension)
   - **Includes**:
     - Send Password Reset Email
     - Validate Reset Token
     - Update Password
   - **Preconditions**: 
     - Customer has registered account with valid email
   - **Postconditions**: 
     - Password reset email sent
     - Password updated (if token valid)
   - **Related Requirements**: FR-045-003
   - **Business Rules**:
     - Reset token expires in 1 hour
     - Reset token can only be used once

**UC-004: Change Password**
   - **Description**: Logged-in customer changes their password
   - **Actors**: Customer
   - **Priority**: Should Have (S)
   - **Preconditions**: 
     - Customer is logged in
   - **Postconditions**: 
     - Password is updated
   - **Related Requirements**: FR-048-001

**Registration Use Cases:**

**UC-005: Register Account**
   - **Description**: New user creates an account
   - **Actors**: Guest User, Email System
   - **Priority**: Must Have (M)
   - **Includes**:
     - Validate Email
     - Validate Password
     - Create Account
     - Send Registration Confirmation
   - **Preconditions**: 
     - User is not registered
     - User has valid email
   - **Postconditions**: 
     - Account is created
     - Confirmation email sent
     - User can login
   - **Related Requirements**: FR-046-001
   - **Business Rules**:
     - Email must be unique
     - Password must meet requirements (8+ chars, etc.)
     - Email verification required (can be done later)

**UC-006: Verify Email**
   - **Description**: Customer verifies email address
   - **Actors**: Customer, Email System
   - **Priority**: Should Have (S)
   - **Preconditions**: 
     - Customer registered but email not verified
   - **Postconditions**: 
     - Email is verified
   - **Related Requirements**: FR-046-002

**Profile Management Use Cases:**

**UC-007: View Profile**
   - **Description**: Customer views their profile information
   - **Actors**: Customer
   - **Priority**: Must Have (M)
   - **Preconditions**: 
     - Customer is logged in
   - **Postconditions**: 
     - Profile information displayed
   - **Related Requirements**: FR-047-001

**UC-008: Update Profile**
   - **Description**: Customer updates profile information
   - **Actors**: Customer
   - **Priority**: Must Have (M)
   - **Includes**:
     - Validate Profile Data
     - Update Profile
   - **Preconditions**: 
     - Customer is logged in
   - **Postconditions**: 
     - Profile information updated
   - **Related Requirements**: FR-047-002
   - **Business Rules**:
     - Email change requires verification
     - Some fields cannot be changed (account creation date)

**UC-009: Upload Profile Picture**
   - **Description**: Customer uploads profile picture
   - **Actors**: Customer
   - **Priority**: Could Have (C)
   - **Preconditions**: 
     - Customer is logged in
   - **Postconditions**: 
     - Profile picture uploaded
   - **Related Requirements**: FR-047-003
   - **Business Rules**:
     - Image size limit: 5MB
     - Supported formats: JPG, PNG
     - Image automatically resized to 200x200px

**Account Settings Use Cases:**

**UC-010: Update Account Settings**
   - **Description**: Customer updates account preferences and settings
   - **Actors**: Customer
   - **Priority**: Should Have (S)
   - **Includes**:
     - Validate Settings
     - Update Settings
   - **Preconditions**: 
     - Customer is logged in
   - **Postconditions**: 
     - Settings updated
   - **Related Requirements**: FR-048-001

**UC-011: Manage Notification Preferences**
   - **Description**: Customer manages email and notification preferences
   - **Actors**: Customer
   - **Priority**: Should Have (S)
   - **Preconditions**: 
     - Customer is logged in
   - **Postconditions**: 
     - Notification preferences updated
   - **Related Requirements**: FR-048-002

**UC-012: Delete Account**
   - **Description**: Customer deletes their account
   - **Actors**: Customer
   - **Priority**: Could Have (C)
   - **Preconditions**: 
     - Customer is logged in
     - Customer confirms deletion
   - **Postconditions**: 
     - Account is deleted (or marked for deletion)
     - Data anonymized (GDPR compliance)
   - **Related Requirements**: FR-048-003
   - **Business Rules**:
     - Requires confirmation
     - 30-day grace period before permanent deletion
     - Active orders prevent deletion

## 4. Relationships & Dependencies

### Include Relationships (Mandatory)

**1. Login <<includes>> Validate Credentials**
   - **Type**: Include (mandatory)
   - **Description**: Login always validates user credentials
   - **Related Requirements**: FR-045-001

**2. Login <<includes>> Create Session**
   - **Type**: Include (mandatory)
   - **Description**: Successful login always creates a session
   - **Related Requirements**: FR-045-001

**3. Register Account <<includes>> Validate Email**
   - **Type**: Include (mandatory)
   - **Description**: Registration always validates email format and uniqueness
   - **Related Requirements**: FR-046-002

**4. Register Account <<includes>> Validate Password**
   - **Type**: Include (mandatory)
   - **Description**: Registration always validates password requirements
   - **Related Requirements**: NFR-002 (Security)

**5. Register Account <<includes>> Create Account**
   - **Type**: Include (mandatory)
   - **Description**: Registration always creates user account
   - **Related Requirements**: FR-046-001

**6. Register Account <<includes>> Send Registration Confirmation**
   - **Type**: Include (mandatory)
   - **Description**: Registration always sends confirmation email
   - **Related Requirements**: FR-046-001

**7. Reset Password <<includes>> Send Password Reset Email**
   - **Type**: Include (mandatory)
   - **Description**: Password reset always sends email
   - **Related Requirements**: FR-045-003

**8. Reset Password <<includes>> Validate Reset Token**
   - **Type**: Include (mandatory)
   - **Description**: Password reset validates token before allowing reset
   - **Related Requirements**: FR-045-003

**9. Reset Password <<includes>> Update Password**
   - **Type**: Include (mandatory)
   - **Description**: Valid password reset always updates password
   - **Related Requirements**: FR-045-003

**10. Update Profile <<includes>> Validate Profile Data**
   - **Type**: Include (mandatory)
   - **Description**: Profile update always validates data
   - **Related Requirements**: FR-047-002

**11. Update Profile <<includes>> Update Profile**
   - **Type**: Include (mandatory)
   - **Description**: Valid profile update always saves changes
   - **Related Requirements**: FR-047-002

### Extend Relationships (Optional)

**1. Login <<extends>> Reset Password**
   - **Type**: Extend (optional)
   - **Description**: User can reset password if they forgot it during login
   - **Condition**: User clicks "Forgot Password" link on login page
   - **Extension Point**: Login page
   - **Related Requirements**: FR-045-003

### Generalization Relationships

**1. Guest User → Customer**
   - **Type**: Generalization (inheritance)
   - **Description**: Guest User becomes Customer after registration
   - **Related Requirements**: FR-046

### Dependencies

**Functional Dependencies**:
- Register Account must complete before Login (user must have account)
- Login must complete before all profile/account use cases (authentication required)
- Reset Password requires valid email (from registration)
- Delete Account requires no active orders

**Technical Dependencies**:
- All use cases depend on authentication infrastructure
- Email use cases depend on Email System integration
- Profile picture upload depends on file storage service
- All use cases depend on database for data persistence

**Critical Path**:
1. Register Account (enables Login)
2. Login (enables all authenticated features)
3. Profile/Account management (depends on Login)

## 5. Business Rules & Constraints

### Authentication Rules

**1. Login Attempts**
   - **Rule**: Maximum 5 failed login attempts before temporary account lockout
   - **Lockout Duration**: 15 minutes
   - **Applies to**: UC-001 (Login)
   - **Related Requirements**: NFR-002 (Security)

**2. Session Management**
   - **Rule**: Session expires after 30 minutes of inactivity
   - **Rule**: Maximum 1 active session per user (new login logs out previous)
   - **Applies to**: UC-001 (Login), UC-002 (Logout)
   - **Related Requirements**: FR-045-004

**3. Password Requirements**
   - **Rule**: Password must be 8+ characters
   - **Rule**: Must include uppercase, lowercase, number, special character
   - **Applies to**: UC-003 (Reset Password), UC-004 (Change Password), UC-005 (Register)
   - **Related Requirements**: NFR-002 (Security)

**4. Password Reset**
   - **Rule**: Reset token expires in 1 hour
   - **Rule**: Reset token can only be used once
   - **Rule**: Maximum 3 password reset requests per hour
   - **Applies to**: UC-003 (Reset Password)
   - **Related Requirements**: FR-045-003, NFR-002 (Security)

### Registration Rules

**5. Email Validation**
   - **Rule**: Email must be valid format
   - **Rule**: Email must be unique (one account per email)
   - **Rule**: Email verification required (can login before verification, but limited features)
   - **Applies to**: UC-005 (Register Account), UC-006 (Verify Email)
   - **Related Requirements**: FR-046-002

**6. Account Creation**
   - **Rule**: Minimum age: 13 years (COPPA compliance)
   - **Rule**: Terms of service acceptance required
   - **Rule**: Privacy policy acceptance required
   - **Applies to**: UC-005 (Register Account)
   - **Related Requirements**: FR-046-001, Legal Requirements

### Profile Rules

**7. Profile Updates**
   - **Rule**: Email change requires verification (new email)
   - **Rule**: Some fields cannot be changed (account creation date, user ID)
   - **Rule**: Profile picture must be < 5MB
   - **Applies to**: UC-008 (Update Profile), UC-009 (Upload Profile Picture)
   - **Related Requirements**: FR-047-002, FR-047-003

**8. Account Deletion**
   - **Rule**: Requires confirmation (double confirmation)
   - **Rule**: 30-day grace period before permanent deletion
   - **Rule**: Active orders prevent deletion
   - **Rule**: Data anonymized per GDPR (not deleted, anonymized)
   - **Applies to**: UC-012 (Delete Account)
   - **Related Requirements**: FR-048-003, Legal Requirements (GDPR)

### Constraints

**Technical Constraints**:
- Must support email and password only (no SSO for MVP)
- Must use HTTPS for all authentication (security requirement)
- Must comply with GDPR (data protection, right to deletion)
- Must support password reset via email only (no SMS for MVP)
- Profile picture storage: Cloud storage (AWS S3 or similar)

**Business Constraints**:
- MVP scope: Email/password only (no social login)
- Email verification: Optional for MVP (can be added later)
- Account deletion: Soft delete with grace period (GDPR compliance)

## 6. Model Validation

### Completeness Check

**Actors**:
- ✅ All user types identified (Customer, Guest User, Admin, Email System)
- ✅ All actors have descriptions
- ✅ All actors linked to use cases

**Use Cases**:
- ✅ All authentication use cases identified
- ✅ All registration use cases identified
- ✅ All profile management use cases identified
- ✅ All account settings use cases identified
- ✅ All use cases have descriptions
- ✅ All use cases linked to requirements

**Relationships**:
- ✅ All include relationships documented
- ✅ All extend relationships documented
- ✅ All generalization relationships documented
- ✅ All dependencies identified

**System Boundary**:
- ✅ System boundary clearly defined
- ✅ External systems identified (Email System)
- ✅ Internal vs external clearly distinguished

### Consistency Check

**Naming**:
- ✅ Use case names consistent with requirements
- ✅ Actor names consistent
- ✅ Relationship labels clear

**Logic**:
- ✅ Relationships logical (no circular dependencies)
- ✅ Preconditions and postconditions consistent
- ✅ Business rules consistent

**Traceability**:
- ✅ All use cases linked to requirements (FR-045, FR-046, FR-047, FR-048)
- ✅ All actors linked to user requirements
- ✅ All business rules linked to requirements

### Stakeholder Review

**Reviewers**:
- Product Owner: ✅ Approved (2024-01-15)
  - Comments: "Comprehensive coverage of user management functionality"
- Development Team: ✅ Approved (2024-01-15)
  - Comments: "Clear use cases, good for implementation planning"
- QA Team: ✅ Approved (2024-01-16)
  - Comments: "Useful for test case development"
- Security Team: ✅ Approved (2024-01-16)
  - Comments: "Security requirements well represented"
- UX Team: ✅ Approved (2024-01-17)
  - Comments: "Good user flow representation"

**Issues Found**: None
**Changes Requested**: None
**Validation Status**: ✅ Validated and Approved

## 7. Model Maintenance

**Version History**:
- v1.0 (2024-01-15): Initial version with core use cases
- v1.1 (2024-01-20): Added "Remember Me" use case (extend Login)
- v1.2 (2024-02-01): Added System Administrator actor and admin use cases
- v1.3 (2024-02-15): Updated business rules based on security review

**Change Log**:
- 2024-01-20: Added "Remember Me" use case (extend Login) - Requested by UX team
- 2024-02-01: Added System Administrator actor and related use cases (View Users, Manage Accounts) - New requirement
- 2024-02-15: Updated password requirements and session timeout rules - Security team feedback

**Update Schedule**: 
- Review monthly
- Update when requirements change
- Update when new use cases identified
- Review after each sprint planning

**Owner**: Business Analyst (Sarah Johnson)
**Co-Owners**: 
- Product Owner (John Smith)
- Technical Lead (Mike Davis)

**Last Review**: 2024-02-15
**Next Review**: 2024-03-15
**Review Frequency**: Monthly or when requirements change

## 8. Tool & Format Information

**Modeling Tool**: Lucidchart
**Tool Version**: Latest (2024)
**File Format**: .lucid (Lucidchart native format)
**Export Formats**: 
- PDF (for documentation) - Primary format
- PNG (for presentations and documents)
- SVG (for web and scalable graphics)
- Visio (for Microsoft Visio compatibility)

**File Locations**: 
- **Cloud**: Lucidchart workspace "E-Commerce Project" / "User Management"
- **Local Backup**: docs/models/use-case-user-management.lucid
- **Documentation**: docs/models/use-case-user-management.pdf
- **Version Control**: Git repository (docs/models/)

**Access Control**: 
- **Team Members**: Full access (edit, comment, view)
- **Stakeholders**: View-only access
- **Public**: Not shared (internal only)

**Collaboration**:
- Real-time collaboration enabled
- Comments and feedback tracked
- Change history maintained
- Notifications for updates

**Integration**:
- Linked to requirements in Jira
- Exported to Confluence for documentation
- Used in presentations (PowerPoint, Google Slides)
```

## How to Find Details for Each Element

### Finding Model Purpose & Scope

**Sources:**
1. **Requirements Documents**: Review requirements
   - Check [Functional Requirements](./Functional%20Requirements.md)
   - Review [Business Requirements](./Business%20Requirements.md)
   - Check [User Requirements](./User%20Requirements.md)
   - Understand modeling objectives

2. **Stakeholder Discussions**: Get modeling needs
   - Review interview notes
   - Check workshop outputs
   - Understand stakeholder needs
   - Identify modeling goals

3. **Project Scope**: Understand boundaries
   - Review [Project Charter](./Project%20Charter.md)
   - Check scope documents
   - Understand system boundaries
   - Identify what to include/exclude

**Tools:**
- **Requirements Management**: Jira, Azure DevOps
- **Documentation**: Confluence, Notion
- **Analysis**: Requirements analysis tools

**Practical Method:**
```markdown
1. Review requirements for modeling needs
2. Identify functional areas to model
3. Define scope and boundaries
4. Identify target audience
5. Document purpose and scope
```

### Finding Model Type & Notation

**Sources:**
1. **Modeling Standards**: Choose appropriate standard
   - UML for system modeling
   - BPMN for business processes
   - ERD for data modeling
   - DFD for data flow

2. **Project Standards**: Follow organizational standards
   - Company modeling standards
   - Team conventions
   - Tool preferences
   - Documentation standards

3. **Requirements Type**: Match model to requirements
   - Use cases for functional requirements
   - Activity diagrams for processes
   - ERD for data requirements
   - State diagrams for state-based requirements

**Tools:**
- **Standards**: UML specification, BPMN specification
- **Tools**: Lucidchart, Draw.io, Enterprise Architect
- **Templates**: Modeling tool templates

**Practical Method:**
```markdown
1. Identify requirements type
2. Select appropriate model type
3. Choose notation standard
4. Select modeling tool
5. Define conventions
```

### Finding Model Elements

**Sources:**
1. **Requirements**: Extract from requirements
   - Functional requirements → Use cases
   - User requirements → Actors
   - Business requirements → Business processes
   - Data requirements → Entities

2. **Stakeholder Input**: Get from stakeholders
   - Review [Structured Interviews](./Structured%20Interviews.md)
   - Review [Unstructured Interviews](./Unstructured%20Interviews.md)
   - Conduct workshops
   - Get user input

3. **Business Processes**: Understand workflows
   - Review [Business Process Document](./Business%20Process%20Document.md)
   - Analyze current processes
   - Identify actors and activities
   - Map workflows

**Tools:**
- **Interviews**: Interview notes, transcripts
- **Workshops**: Miro, Mural, whiteboards
- **Process Analysis**: Process mapping tools

**Practical Method:**
```bash
# Extract use cases from requirements
grep -r "system shall\|user can\|system must" docs/requirements/
# Identify actors from user requirements
grep -r "user\|actor\|stakeholder" docs/user-requirements/
# Extract business processes
grep -r "process\|workflow\|activity" docs/business-process/
```

### Finding Relationships & Dependencies

**Sources:**
1. **Requirement Dependencies**: Map relationships
   - Review [Requirements Prioritization](./Requirements%20Prioritization.md)
   - Check requirement dependencies
   - Analyze functional dependencies
   - Map relationships

2. **Functional Analysis**: Understand interactions
   - Analyze use case interactions
   - Identify include/extend relationships
   - Map dependencies
   - Understand flows

3. **Technical Dependencies**: Consider technical aspects
   - Review architecture
   - Check technical dependencies
   - Understand system integration
   - Map technical relationships

**Tools:**
- **Dependency Mapping**: Draw.io, Lucidchart
- **Analysis**: Dependency matrices
- **Requirements Management**: Jira, Azure DevOps (links)

**Practical Method:**
```markdown
1. Review requirements for dependencies
2. Analyze use case interactions
3. Map include/extend relationships
4. Identify generalization relationships
5. Document all relationships
```

### Finding Business Rules & Constraints

**Sources:**
1. **Business Requirements**: Review business rules
   - Check [Business Requirements](./Business%20Requirements.md)
   - Review [Business Process Document](./Business%20Process%20Document.md)
   - Analyze business logic
   - Extract rules

2. **Stakeholder Input**: Get from stakeholders
   - Business stakeholders
   - Domain experts
   - Process owners
   - Compliance team

3. **Regulations**: Consider compliance
   - GDPR, HIPAA, PCI DSS
   - Industry regulations
   - Legal requirements
   - Compliance rules

**Tools:**
- **Business Analysis**: Business rule repositories
- **Compliance**: Compliance documentation
- **Documentation**: Business rule templates

**Practical Method:**
```markdown
1. Review business requirements
2. Extract business rules
3. Identify constraints
4. Document preconditions/postconditions
5. Map to use cases/processes
```

### Finding Model Validation

**Sources:**
1. **Validation Criteria**: Define criteria
   - Completeness checklist
   - Consistency rules
   - Traceability requirements
   - Quality standards

2. **Stakeholder Review**: Get feedback
   - Present to stakeholders
   - Collect feedback
   - Address issues
   - Get approvals

3. **Peer Review**: Technical review
   - Development team review
   - Architecture team review
   - QA team review
   - Security team review

**Tools:**
- **Review**: Review tools, collaboration platforms
- **Validation**: Checklists, validation tools
- **Tracking**: Issue tracking, feedback tools

**Practical Method:**
```markdown
1. Define validation criteria
2. Conduct completeness check
3. Conduct consistency check
4. Review with stakeholders
5. Get approvals
6. Document validation
```

### Finding Model Maintenance

**Sources:**
1. **Change Management**: Track changes
   - Version control
   - Change logs
   - Update procedures
   - Review schedules

2. **Requirements Changes**: Respond to changes
   - Monitor requirement changes
   - Update models accordingly
   - Maintain traceability
   - Document changes

**Tools:**
- **Version Control**: Git, SVN
- **Change Tracking**: Change logs, version history
- **Documentation**: Documentation tools

**Practical Method:**
```markdown
1. Set up version control
2. Document changes
3. Set review schedule
4. Assign ownership
5. Track maintenance
```

### Finding Tool & Format Information

**Sources:**
1. **Tool Selection**: Choose modeling tool
   - Review [Tool Selection](./Tool%20Selection.md)
   - Evaluate tools
   - Consider team preferences
   - Check organizational standards

2. **Format Requirements**: Define formats
   - Documentation formats
   - Presentation formats
   - Export formats
   - Access requirements

**Tools:**
- **Modeling Tools**: Lucidchart, Draw.io, Enterprise Architect, Visio
- **Export**: PDF, PNG, SVG, various formats
- **Storage**: Cloud storage, version control

**Practical Method:**
```markdown
1. Select modeling tool
2. Define file formats
3. Set up storage/access
4. Configure exports
5. Document tool information
```

## Practical Tools for Requirements Modeling

### UML Modeling Tools

**Cloud-Based:**
- **Lucidchart**: Web-based, collaborative UML modeling
- **Draw.io (diagrams.net)**: Free, open-source diagramming
- **Creately**: Online diagramming and collaboration
- **Gliffy**: Simple diagramming tool

**Desktop:**
- **Enterprise Architect**: Comprehensive UML modeling
- **Visual Paradigm**: Professional UML tool
- **StarUML**: Free UML modeling tool
- **ArgoUML**: Open-source UML tool

**Specialized:**
- **PlantUML**: Text-based UML diagrams
  ```plantuml
  @startuml
  actor User
  User --> (Login)
  @enduml
  ```
- **Mermaid**: Markdown-based diagrams
  ```mermaid
  graph TD
    A[User] --> B[Login]
  ```

### BPMN Tools

- **Camunda Modeler**: Free BPMN modeling
- **Bizagi Modeler**: Business process modeling
- **Signavio**: Process modeling and management
- **Trisotech**: BPMN modeling tool

### Data Modeling Tools

- **dbdiagram.io**: Database diagram tool
- **ERDPlus**: Entity relationship diagrams
- **MySQL Workbench**: Database design
- **pgAdmin**: PostgreSQL database tool

### General Diagramming Tools

- **Miro**: Collaborative whiteboard
- **Mural**: Digital workspace
- **Figma**: Design and diagramming
- **Whimsical**: Simple diagramming

### Code-Based Modeling

- **PlantUML**: Text-based UML
  ```bash
  # Install PlantUML
  npm install -g node-plantuml
  # Generate diagram
  plantuml diagram.puml
  ```

- **Mermaid**: Markdown diagrams
  ```bash
  # Use in Markdown
  ```mermaid
  graph TD
    A --> B
  ```
  ```

- **Graphviz**: Graph visualization
  ```bash
  # Install Graphviz
  brew install graphviz
  # Generate diagram
  dot -Tpng diagram.dot -o diagram.png
  ```

## Practical Workflow: Step-by-Step

### Step 1: Identify Modeling Needs

**Activities:**
1. Review requirements
2. Identify areas needing modeling
3. Determine model types needed
4. Define modeling objectives
5. Identify stakeholders

**Output:** Modeling plan

**Time:** 2-4 hours

### Step 2: Select Tools & Standards

**Activities:**
1. Choose modeling tool
2. Select notation standards
3. Define conventions
4. Set up tool access
5. Create templates

**Output:** Tool setup and standards

**Time:** 1-2 hours

### Step 3: Create Initial Models

**Activities:**
1. Identify actors/elements
2. Create use cases/activities
3. Draw initial diagrams
4. Add relationships
5. Document elements

**Output:** Initial models

**Time:** 4-8 hours per model

### Step 4: Refine & Validate

**Activities:**
1. Review with stakeholders
2. Refine models
3. Validate completeness
4. Check consistency
5. Get approvals

**Output:** Validated models

**Time:** 2-4 hours per model

### Step 5: Document & Maintain

**Activities:**
1. Document all elements
2. Create model documentation
3. Set up version control
4. Establish maintenance process
5. Schedule reviews

**Output:** Documented models with maintenance plan

**Time:** 2-4 hours

**Total Time:** 11-22 hours per model (typically 1-3 days)

## Best Practices

### Do's

✅ **Use Standard Notations**
- Use UML, BPMN, or other standards
- Follow notation conventions
- Use consistent symbols
- Document conventions

✅ **Keep Models Simple**
- Focus on essential elements
- Avoid over-complication
- Use appropriate level of detail
- Group related elements

✅ **Maintain Traceability**
- Link models to requirements
- Document relationships
- Keep models updated
- Track changes

✅ **Involve Stakeholders**
- Get stakeholder input
- Review with users
- Validate with experts
- Get approvals

✅ **Document Thoroughly**
- Document all elements
- Explain relationships
- Document business rules
- Maintain version history

### Don'ts

❌ **Don't Over-Model**
- Don't model everything
- Focus on important areas
- Avoid unnecessary detail
- Keep it practical

❌ **Don't Ignore Standards**
- Use standard notations
- Follow conventions
- Don't invent new symbols
- Maintain consistency

❌ **Don't Skip Validation**
- Validate with stakeholders
- Check completeness
- Verify consistency
- Get approvals

❌ **Don't Forget Maintenance**
- Keep models updated
- Respond to changes
- Maintain version control
- Review regularly

❌ **Don't Work in Isolation**
- Involve stakeholders
- Get team input
- Collaborate
- Share models

## Common Pitfalls & How to Avoid Them

### Pitfall 1: Over-Complication

**Problem:** Models too complex, hard to understand

**Solution:**
- Keep models simple
- Focus on essential elements
- Use appropriate detail level
- Group related elements

### Pitfall 2: Inconsistent Notation

**Problem:** Using different symbols/conventions

**Solution:**
- Use standard notations
- Define conventions
- Create style guide
- Review for consistency

### Pitfall 3: Missing Traceability

**Problem:** Models not linked to requirements

**Solution:**
- Link models to requirements
- Document relationships
- Maintain traceability matrix
- Update when requirements change

### Pitfall 4: Not Validating

**Problem:** Models not reviewed with stakeholders

**Solution:**
- Review with stakeholders
- Validate completeness
- Check consistency
- Get approvals

### Pitfall 5: Not Maintaining

**Problem:** Models become outdated

**Solution:**
- Keep models updated
- Respond to changes
- Maintain version control
- Review regularly

## Integration with Requirements Process

Requirements Modeling is part of the complete requirements process:

1. **Requirements Elicitation**: Gather requirements
2. **Requirements Analysis**: Analyze requirements
3. **Requirements Modeling**: Create visual models ← **You are here**
4. **Requirements Validation**: Validate requirements
5. **Requirements Management**: Manage requirements

See [Planning & Requirements Gathering](./Planning%20&%20Requirements%20Gathering.md) for the complete requirements process.

## Relationship with Other Requirements Activities

**Requirements Categorization**: Groups requirements by type
**Requirements Prioritization**: Ranks requirements by importance
**Requirements Modeling**: Visualizes requirements with diagrams

**Example:**
- **Categorization**: Functional, Non-Functional
- **Prioritization**: Must Have, Should Have
- **Modeling**: Use Case Diagram showing functional requirements

All work together for comprehensive requirements management.

## Conclusion

Requirements Modeling is essential for:
- **Understanding** requirements better through visualization
- **Communicating** with stakeholders using common language
- **Identifying** gaps and inconsistencies
- **Validating** requirements completeness
- **Designing** systems based on requirements

Key success factors:
- ✅ Use standard notations
- ✅ Keep models simple
- ✅ Maintain traceability
- ✅ Involve stakeholders
- ✅ Document thoroughly
- ✅ Validate and review
- ✅ Maintain and update

Remember: Models are tools for understanding and communication. They should be clear, accurate, and maintained. Effective modeling helps ensure requirements are well-understood and correctly implemented.

