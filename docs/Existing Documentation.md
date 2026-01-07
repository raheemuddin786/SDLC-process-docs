---
title: "Existing Documentation - Detailed Guide"
description: "Comprehensive guide to Document Analysis: Review current systems and processes"
author: "Development Team"
date: "2024"
---

# Existing Documentation: Review Current Systems

## Overview

**Existing Documentation Analysis** is a requirements gathering technique that involves reviewing and analyzing current system documentation, business process documents, legacy system documentation, and other relevant materials to understand the current state, identify requirements, and learn from existing implementations.

## Definition

Document Analysis is:
- **Systematic review** of existing documentation
- **Understanding current state** through documents
- **Requirements discovery** from existing systems
- **Learning from legacy** systems and processes
- **Foundation building** for new requirements

## Key Characteristics

### Non-Intrusive
- Doesn't require stakeholder time
- Can be done independently
- No scheduling needed
- Efficient use of time

### Comprehensive
- Covers multiple aspects
- Historical perspective
- Complete picture
- Context-rich

### Cost-Effective
- Low cost method
- Reuses existing information
- No additional data collection
- Quick to start

### Foundation-Building
- Understands current state
- Identifies gaps
- Learns from past
- Informs new requirements

## Types of Documents to Review

### 1. System Documentation
- **Technical Specifications**: System architecture, APIs
- **User Manuals**: How current system works
- **Admin Guides**: System administration
- **API Documentation**: Integration points
- **Database Schemas**: Data structure

### 2. Business Process Documents
- **Process Flows**: Business workflows
- **Standard Operating Procedures (SOPs)**: How things are done
- **Policy Documents**: Business rules and policies
- **Work Instructions**: Step-by-step procedures
- **Business Rules**: Decision logic

### 3. Legacy System Documentation
- **System Requirements**: Old requirements
- **Design Documents**: Architecture decisions
- **Change Logs**: System evolution
- **Known Issues**: Problems and limitations
- **Migration Notes**: Previous migration experiences

### 4. Project Documentation
- **Previous Project Plans**: Past implementations
- **Requirements Documents**: Historical requirements
- **Test Plans**: Testing approaches
- **Lessons Learned**: What worked/didn't work
- **Post-Mortems**: Project reviews

### 5. User Documentation
- **Training Materials**: How users are trained
- **FAQ Documents**: Common questions
- **Help Guides**: User assistance
- **Video Tutorials**: User workflows
- **Knowledge Base Articles**: User information

### 6. Compliance & Regulatory
- **Compliance Documents**: Regulatory requirements
- **Audit Reports**: Compliance findings
- **Security Policies**: Security requirements
- **Data Privacy Documents**: Privacy requirements
- **Industry Standards**: Standards compliance

## How to Find Existing Documentation

### 1. Internal Sources

#### Document Repositories
- **Shared Drives**: Network drives, SharePoint
- **Document Management Systems**: Confluence, SharePoint, Documentum
- **Wiki Systems**: Internal wikis, knowledge bases
- **Version Control**: Git repositories with docs
- **File Servers**: Company file servers

**How to Find**:
- Ask IT department for access
- Check company intranet
- Search document management systems
- Review shared folders
- Check team wikis

#### Department Resources
- **IT Department**: Technical documentation
- **Business Units**: Process documentation
- **Compliance Team**: Regulatory documents
- **Training Department**: Training materials
- **Support Team**: User guides, FAQs

**How to Find**:
- Contact department heads
- Request documentation access
- Ask for document inventories
- Review department wikis
- Check department shared folders

#### Project Archives
- **Project Folders**: Previous project documentation
- **Archive Systems**: Archived project files
- **Lessons Learned Repositories**: Project reviews
- **PMO Documentation**: Project management office files

**How to Find**:
- Contact PMO (Project Management Office)
- Review project archives
- Check project management tools
- Ask previous project managers
- Review lessons learned databases

### 2. External Sources

#### Vendor Documentation
- **Software Vendors**: Product documentation
- **System Integrators**: Implementation docs
- **Consultants**: Deliverables from past projects
- **Third-Party Providers**: Service documentation

**How to Find**:
- Contact vendor support
- Review vendor portals
- Check contract deliverables
- Request from procurement
- Review vendor websites

#### Industry Resources
- **Industry Standards**: ISO, IEEE standards
- **Best Practices**: Industry guides
- **Regulatory Bodies**: Compliance requirements
- **Professional Associations**: Industry documentation

**How to Find**:
- Search industry standards websites
- Review regulatory body websites
- Check professional association resources
- Consult industry experts
- Review compliance databases

### 3. System Sources

#### Application Systems
- **Help Systems**: Built-in help documentation
- **System Metadata**: Database schemas, configurations
- **Log Files**: System behavior documentation
- **Configuration Files**: System settings

**How to Find**:
- Access system help menus
- Review system documentation features
- Export system metadata
- Analyze configuration files
- Review system logs

#### Code Repositories
- **Source Code**: Code comments, README files
- **Version Control**: Commit messages, change logs
- **Documentation Folders**: In-repo documentation
- **API Documentation**: Code-generated docs

**How to Find**:
- Access version control systems (Git, SVN)
- Review code repositories
- Check documentation folders
- Review commit history
- Generate API documentation

## Complete Example: Customer Portal Document Analysis

### Project Context
**Project**: Customer Self-Service Portal Development
**Objective**: Understand current customer support systems and processes
**Timeline**: 2 weeks for document analysis
**Team**: Business Analyst, Technical Lead

### Document Discovery Process

#### Step 1: Identify Document Sources

**Internal Sources Identified**:
1. IT Department - Technical documentation
2. Customer Service Department - Process documentation
3. Training Department - User training materials
4. Compliance Team - Regulatory requirements
5. Previous Projects - Legacy system docs

**External Sources Identified**:
1. Current CRM Vendor - System documentation
2. Ticketing System Vendor - User guides
3. Industry Standards - Customer service standards

#### Step 2: Document Inventory

**Document Collection Checklist**:

| Document Type | Source | Location | Status | Notes |
|---------------|--------|----------|--------|-------|
| Current CRM System Spec | IT Dept | SharePoint/Systems/CRM | ✅ Found | Version 3.2 |
| Customer Service SOP | CS Dept | SharePoint/Processes | ✅ Found | Last updated 2023 |
| Ticketing System Guide | Vendor Portal | support.ticketsys.com | ✅ Found | Requires login |
| Training Materials | Training Dept | Learning Management System | ✅ Found | 15 modules |
| API Documentation | IT Dept | Confluence/APIs | ✅ Found | REST API v2 |
| Database Schema | IT Dept | Git Repo | ✅ Found | MySQL schema |
| Previous Portal Project | PMO | Project Archive | ✅ Found | 2019 project |
| Compliance Requirements | Compliance | SharePoint/Compliance | ✅ Found | GDPR, PCI-DSS |
| User Manuals | Support Team | Knowledge Base | ✅ Found | 50+ articles |
| Business Rules Document | Business Ops | SharePoint/Business | ✅ Found | 2024 version |

---

### Document Analysis: Current CRM System Specification

#### Document Details
- **Document Name**: Customer Relationship Management System - Technical Specification v3.2
- **Source**: IT Department
- **Date**: March 2023
- **Author**: System Architect Team
- **Location**: SharePoint/Systems/CRM/Specifications
- **Pages**: 145 pages
- **Status**: Current (Active)

#### Key Sections Analyzed

**Section 1: System Overview**

**Content Extracted**:
```
The CRM system manages customer information, order history, 
communication logs, and support tickets. It serves 500+ 
customer service representatives and handles 50,000+ 
customer interactions monthly.

Key Modules:
- Customer Profile Management
- Order Tracking
- Communication History
- Ticket Management
- Reporting & Analytics
```

**Requirements Identified**:
- System must handle 50,000+ monthly interactions
- Support for 500+ concurrent users
- Customer profile management required
- Order tracking functionality needed
- Communication history tracking essential

**Gaps Identified**:
- No customer self-service capability
- All interactions require agent involvement
- Limited customer-facing features

---

**Section 2: Customer Data Model**

**Content Extracted**:
```
Customer Entity:
- Customer ID (Primary Key)
- Name, Email, Phone
- Address (Billing, Shipping)
- Account Status (Active, Inactive, Suspended)
- Registration Date
- Last Login Date
- Customer Tier (Standard, Premium, VIP)
- Preferences (Language, Communication)

Order Entity:
- Order ID
- Customer ID (Foreign Key)
- Order Date
- Order Status (Pending, Processing, Shipped, Delivered, Cancelled)
- Total Amount
- Shipping Address
- Tracking Number
- Items (Line Items)
```

**Requirements Identified**:
- Customer data structure: ID, contact info, addresses, status, tier
- Order data: ID, status, dates, amounts, tracking
- Customer preferences: Language, communication
- Customer tiers: Standard, Premium, VIP (different service levels)

**Data Requirements**:
- Customer profile display
- Order history viewing
- Order status tracking
- Address management
- Preference management

---

**Section 3: API Endpoints**

**Content Extracted**:
```
GET /api/v2/customers/{customerId}
  Returns: Customer profile information
  Authentication: Required (API Key)
  Rate Limit: 100 requests/minute

GET /api/v2/customers/{customerId}/orders
  Returns: List of customer orders
  Parameters: status, dateRange, limit
  Authentication: Required

GET /api/v2/orders/{orderId}/tracking
  Returns: Order tracking information
  Authentication: Required

POST /api/v2/tickets
  Creates: New support ticket
  Body: {subject, description, priority, category}
  Authentication: Required
```

**Requirements Identified**:
- API integration available for customer data
- Order information accessible via API
- Ticket creation possible via API
- Authentication required (API Key)
- Rate limiting in place (100 req/min)

**Integration Requirements**:
- Portal must integrate with CRM API
- API authentication needed
- Rate limiting considerations
- API version: v2 (current)

---

**Section 4: Current Limitations**

**Content Extracted**:
```
Known Limitations:
1. No customer self-service portal
2. All customer interactions require agent
3. Limited mobile support (web interface not mobile-optimized)
4. API rate limits may restrict high-volume operations
5. Real-time order updates have 5-minute delay
6. Customer cannot update own profile information
7. No customer-facing knowledge base
8. Password reset requires agent intervention
```

**Requirements Identified** (from limitations):
- Self-service portal needed (addresses limitation #1)
- Mobile-responsive design required (addresses #3)
- Real-time updates preferred (addresses #5)
- Customer profile editing needed (addresses #6)
- Knowledge base required (addresses #7)
- Automated password reset needed (addresses #8)

---

### Document Analysis: Customer Service Standard Operating Procedures

#### Document Details
- **Document Name**: Customer Service Standard Operating Procedures v2.1
- **Source**: Customer Service Department
- **Date**: January 2024
- **Author**: Customer Service Management
- **Location**: SharePoint/Processes/CustomerService/SOP
- **Pages**: 78 pages
- **Status**: Current (Active)

#### Key Sections Analyzed

**Section 1: Inquiry Handling Process**

**Content Extracted**:
```
Process Flow:
1. Customer contacts support (phone/email/chat)
2. Agent greets and identifies customer
3. Agent accesses CRM to view customer profile
4. Agent identifies inquiry type:
   a. Order Status (40% of inquiries)
   b. Account Issues (25% of inquiries)
   c. Product Questions (20% of inquiries)
   d. Billing Questions (10% of inquiries)
   e. Technical Support (5% of inquiries)
5. Agent resolves inquiry or escalates
6. Agent documents interaction in CRM
7. Agent closes ticket

Average Handling Time:
- Order Status: 3-5 minutes
- Account Issues: 5-10 minutes
- Product Questions: 5-15 minutes
- Billing Questions: 10-20 minutes
- Technical Support: 15-30 minutes
```

**Requirements Identified**:
- Inquiry types: Order status (40%), Account (25%), Product (20%), Billing (10%), Technical (5%)
- Order status inquiries are highest volume (40%)
- Average handling times vary by type
- Documentation of interactions required
- Ticket creation and tracking needed

**Portal Requirements**:
- Order status checking (addresses 40% of inquiries)
- Account management (addresses 25% of inquiries)
- Product information/knowledge base (addresses 20% of inquiries)
- Billing information access (addresses 10% of inquiries)

---

**Section 2: Customer Identification Requirements**

**Content Extracted**:
```
Customer Identification Process:
- Verify customer identity before providing information
- Required information for verification:
  * Full name
  * Email address OR phone number
  * Last 4 digits of order number OR account number
- For account changes, additional verification required:
  * Security question answer
  * OR recent order details
- Document all verification attempts
```

**Requirements Identified**:
- Customer authentication required
- Multiple verification methods needed
- Security questions for sensitive operations
- Audit trail for verification attempts
- Different security levels for different operations

**Security Requirements**:
- Multi-factor authentication for account changes
- Security questions implementation
- Audit logging
- Identity verification process

---

**Section 3: Escalation Procedures**

**Content Extracted**:
```
Escalation Triggers:
- Billing disputes over $500
- Order issues requiring refund
- Technical issues beyond agent knowledge
- VIP customer complaints
- Security concerns

Escalation Process:
1. Agent identifies escalation need
2. Agent creates escalation ticket
3. Ticket assigned to appropriate department
4. Customer notified of escalation
5. Follow-up within 24 hours required
```

**Requirements Identified**:
- Escalation functionality needed
- Different escalation paths for different issues
- Customer notification required
- Follow-up tracking needed
- VIP customer special handling

**Portal Requirements**:
- Ticket submission with priority/category
- Escalation request capability
- Status tracking for escalated tickets
- VIP customer identification and handling

---

### Document Analysis: Previous Portal Project Documentation

#### Document Details
- **Document Name**: Customer Portal Project - Lessons Learned Report
- **Source**: PMO Archive
- **Date**: December 2019
- **Project Status**: Cancelled (Phase 1 incomplete)
- **Location**: Project Archive/2019/CustomerPortal
- **Pages**: 45 pages

#### Key Findings

**What Was Attempted**:
- Basic customer portal with order tracking
- Account management features
- Integration with CRM system
- Timeline: 6 months, Budget: $300,000

**Why It Failed**:
1. **Poor User Experience**: Portal was difficult to navigate, customers didn't use it
2. **Slow Performance**: Page load times exceeded 5 seconds
3. **Limited Features**: Only order tracking, customers still needed to call for other needs
4. **Mobile Issues**: Not mobile-responsive, poor mobile experience
5. **Integration Problems**: CRM API integration had issues, data sync delays
6. **Low Adoption**: Only 15% of customers used portal after 6 months

**What Worked**:
- Order tracking feature was appreciated by users who tried it
- Integration approach was sound (API-based)
- Security implementation was successful

**Recommendations from Report**:
1. Prioritize user experience and ease of use
2. Ensure fast performance (<2 seconds load time)
3. Include comprehensive features (not just order tracking)
4. Mobile-first design approach
5. Thorough API integration testing
6. User adoption strategy needed

**Requirements Identified** (Learning from Failure):
- User experience must be excellent (critical success factor)
- Performance must be fast (<2 seconds)
- Comprehensive feature set needed
- Mobile-responsive design essential
- Robust API integration required
- User adoption strategy needed

---

### Document Analysis: API Documentation

#### Document Details
- **Document Name**: CRM REST API v2.0 Documentation
- **Source**: IT Department / Confluence
- **Date**: February 2024
- **Location**: Confluence/APIs/CRM-API
- **Format**: Online documentation

#### Key Information Extracted

**Authentication**:
```
Method: API Key
Header: X-API-Key: {api_key}
Rate Limit: 100 requests per minute per key
```

**Available Endpoints**:
```
GET /api/v2/customers/{id}
GET /api/v2/customers/{id}/orders
GET /api/v2/orders/{id}
GET /api/v2/orders/{id}/tracking
POST /api/v2/tickets
GET /api/v2/tickets/{id}
GET /api/v2/tickets/{id}/history
```

**Data Formats**:
- Request: JSON
- Response: JSON
- Error Format: Standardized error responses

**Integration Requirements**:
- API Key authentication
- Rate limiting: 100 req/min
- JSON data format
- RESTful API design
- Version: v2.0

---

### Document Analysis Summary

#### Requirements Discovered

**Functional Requirements**:
1. Order tracking (40% of inquiries)
2. Account management (25% of inquiries)
3. Product information/knowledge base (20% of inquiries)
4. Billing information access (10% of inquiries)
5. Ticket submission and tracking
6. Customer profile viewing and editing
7. Password reset automation
8. Address management
9. Communication history viewing

**Non-Functional Requirements**:
1. Performance: <2 seconds page load (learned from previous failure)
2. Mobile-responsive design (critical)
3. Support 50,000+ monthly interactions
4. Support 500+ concurrent users
5. API integration with CRM system
6. Rate limiting considerations (100 req/min)
7. Security: Multi-factor authentication for sensitive operations
8. User experience: Easy navigation (critical success factor)

**Technical Requirements**:
1. Integration with CRM API v2.0
2. API Key authentication
3. JSON data format
4. Real-time data (address 5-minute delay limitation)
5. Audit logging for security

**Business Requirements**:
1. Reduce order status inquiries (40% of volume)
2. Enable customer self-service
3. Improve customer satisfaction
4. Reduce agent workload
5. Support VIP customer handling

---

## Document Analysis Template

### Document Analysis Form

**Document Information**:
- **Document Name**: _______________
- **Source**: _______________
- **Date**: _______________
- **Author**: _______________
- **Location**: _______________
- **Version**: _______________
- **Status**: _______________

**Analysis Details**:
- **Analyst**: _______________
- **Analysis Date**: _______________
- **Time Spent**: _______________

**Key Sections Reviewed**:
1. _______________
2. _______________
3. _______________

**Requirements Identified**:
1. _______________
2. _______________
3. _______________

**Gaps Identified**:
1. _______________
2. _______________
3. _______________

**Limitations Found**:
1. _______________
2. _______________
3. _______________

**Integration Points**:
1. _______________
2. _______________
3. _______________

**Key Insights**:
- _______________
- _______________
- _______________

**Follow-up Actions**:
- [ ] Verify with stakeholders
- [ ] Clarify unclear points
- [ ] Request additional documentation
- [ ] Schedule follow-up meetings

---

## Document Discovery Checklist

### Internal Sources
- [ ] IT Department documentation
- [ ] Business unit process documents
- [ ] Training materials
- [ ] Compliance documentation
- [ ] Previous project archives
- [ ] PMO documentation
- [ ] Department wikis
- [ ] Shared drives
- [ ] Document management systems
- [ ] Code repositories

### External Sources
- [ ] Vendor documentation
- [ ] Industry standards
- [ ] Regulatory requirements
- [ ] Third-party system docs
- [ ] Consultant deliverables

### System Sources
- [ ] Application help systems
- [ ] System metadata
- [ ] Configuration files
- [ ] API documentation
- [ ] Database schemas

---

## Best Practices

### Document Discovery
- ✅ Start with stakeholder interviews to identify sources
- ✅ Create document inventory early
- ✅ Request access proactively
- ✅ Use multiple search methods
- ✅ Check both digital and physical archives
- ✅ Verify document currency/version

### Document Analysis
- ✅ Read systematically (section by section)
- ✅ Take detailed notes
- ✅ Extract specific requirements
- ✅ Identify gaps and limitations
- ✅ Note integration points
- ✅ Document source for traceability

### Verification
- ✅ Validate findings with stakeholders
- ✅ Clarify unclear information
- ✅ Update outdated information
- ✅ Cross-reference multiple documents
- ✅ Verify current system state

### Common Mistakes to Avoid
- ❌ Assuming documents are current
- ❌ Not verifying information
- ❌ Missing important documents
- ❌ Not documenting sources
- ❌ Ignoring limitations
- ❌ Not following up on gaps

## Advantages & Disadvantages

### Advantages
- ✅ Non-intrusive (no stakeholder time)
- ✅ Cost-effective
- ✅ Comprehensive coverage
- ✅ Historical perspective
- ✅ Quick to start
- ✅ Context-rich information

### Disadvantages
- ❌ Documents may be outdated
- ❌ May miss undocumented processes
- ❌ Requires verification
- ❌ Can be time-consuming to read
- ❌ May not reflect current reality
- ❌ Limited to what's documented

## Conclusion

Document Analysis is effective for:
- **Understanding**: Current state and context
- **Discovery**: Requirements and constraints
- **Learning**: From previous implementations
- **Foundation**: Building requirements base
- **Efficiency**: Non-intrusive data collection

Well-conducted Document Analysis:
- Provides comprehensive understanding
- Identifies requirements and gaps
- Learns from past experiences
- Informs new requirements
- Supports requirements validation

Remember: Document analysis should be combined with other techniques (interviews, workshops) to validate findings and fill gaps. Always verify document currency and cross-reference information.
