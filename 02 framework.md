## Complete SDL Phase Overview

### **A1: Security Assessment Phase**

**Competency**: Assessing software requirements and risks

**Key Success Factors:**

- Accuracy of planned SDL activities
- Product risk profile understanding
- Accurate threat profile
- Coverage of regulations/compliance
- Security objectives coverage

**Key Deliverables:**

- Product risk profile
- SDL project outline
- Applicable laws and regulations
- Threat profile
- Certification requirements
- Third-party software list
- Metrics template

### **A2: Architecture Phase**

**Competency**: Examining security principles within SDLC

**Key Success Factors:**

- Business requirements and risks identification (CIA)
- Effective threat modeling
- Architectural threat analysis
- Risk mitigation strategy
- DFD accuracy

**Key Deliverables:**

- Business requirements
- Threat modeling artifacts (DFDs, elements, threats)
- Architecture threat analysis
- Risk mitigation plan
- Policy compliance analysis

### **A3: Design & Development Phase**

**Competency**: Evaluating software security test plan

**Key Success Factors:**

- Comprehensive security test plan
- Effective threat modeling (continued)
- Design security analysis
- Privacy implementation assessment
- Policy compliance review updates

**Key Deliverables:**

- Updated threat modeling artifacts
- Design security review
- Security test plans
- Updated policy compliance analysis
- Privacy implementation assessment results

### **A4: Readiness Phase**

**Competency**: Evaluating effectiveness of software testing

**Key Success Factors:**

- Security test case execution
- Security testing completion
- Privacy validation and remediation
- Policy compliance review

**Key Deliverables:**

- Security test execution report
- Updated policy compliance analysis
- Privacy compliance report
- Security testing reports
- Remediation report

### **A5: Ship Phase**

**Final release preparation**

**Key Success Factors:**

- Final policy compliance analysis
- Vulnerability scanning
- Penetration testing
- Open-source licensing review
- Final security review
- Final privacy review
- Customer engagement framework

**Key Deliverables:**

- Updated policy compliance analysis
- Security testing reports
- Remediation report
- Open-source licensing review report
- Final security and privacy review reports
- Customer engagement framework

### **PRS: Post-Release Support**

**Ongoing maintenance and response**

**Key Deliverables:**

- External vulnerability disclosure response process
- Post-release certifications
- Third-party security reviews
- Security strategy for legacy code, M&A, and EOL plans

---

## Critical Exam Overlap & Conflict Analysis

### **HIGH-RISK CONFUSION AREAS**

|**Concept**|**Context Variations**|**Exam Risk**|
|---|---|---|
|**Threat Modeling**|A2: Initial modeling<br>A3: Updated artifacts<br>Tools: STRIDE vs PASTA vs DREAD|**HIGH** - Appears in multiple phases with different purposes|
|**Policy Compliance Analysis**|A2: Initial analysis<br>A3: Updates<br>A4: Compliance review<br>A5: Final analysis|**HIGH** - Same name, different stages|
|**Security Testing**|A3: Test planning<br>A4: Test execution<br>A5: Final testing|**HIGH** - Planning vs execution vs validation|
|**Privacy Activities**|A3: Implementation assessment<br>A4: Validation/remediation<br>A5: Final review|**MEDIUM** - Progressive privacy validation|
|**Risk Mitigation**|A2: Risk mitigation plan<br>A3: Test plans to mitigate risk|**MEDIUM** - Different contexts for same goal|

### **METHODOLOGY DISTINCTIONS**

|**Framework**|**Purpose**|**Key Differentiator**|
|---|---|---|
|**STRIDE**|Threat categorization|Spoofing, Tampering, Repudiation, Information Disclosure, Denial of Service, Elevation of Privilege|
|**PASTA**|Threat modeling process|Process for Attack Simulation and Threat Analysis|
|**DREAD**|Risk scoring|Damage, Reproducibility, Exploitability, Affected users, Discoverability|
|**BSIMM**|Maturity assessment|Studies real-world security initiatives|
|**SAMM**|Prescriptive framework|Software Assurance Maturity Model|

### **TESTING TYPE CONFUSION**

|**Testing Type**|**Information Access**|**When Used**|
|---|---|---|
|**White-box**|Full source code + documentation|A3/A4 - Comprehensive internal testing|
|**Black-box**|No internal knowledge|A4/A5 - External perspective testing|
|**Gray-box**|Limited internal knowledge|A4 - Hybrid approach|
|**Static Analysis**|Code without execution|A3/A4 - SAST tools like SonarQube|
|**Dynamic Analysis**|Runtime execution|A4/A5 - DAST tools, penetration testing|

### **ROLE RESPONSIBILITIES**

|**Role**|**Primary Function**|**Key Activities**|
|---|---|---|
|**Software Security Architect**|Design secure frameworks|Creates secure coding practices, methodologies|
|**Security Champion**|Advocate/promote|Promotes security within development teams|
|**Scrum Master**|Facilitate process|Removes impediments, facilitates ceremonies|
|**Software Developer**|Implement features|Writes code, attends ceremonies|

### **AGILE SDL REQUIREMENTS**

|**Requirement Type**|**Application**|**Example**|
|---|---|---|
|**Every-sprint**|Universal practices|Input validation for all user input|
|**Bucket**|Feature-specific|RPC fuzz testing when RPC implemented|
|**One-time**|Project setup|Initial threat modeling framework|
|**Final review**|Release gates|Comprehensive security assessment|

### **CRITICAL TERMINOLOGY DISTINCTIONS**

- **SDL vs SDLC**: SDL = Security Development Lifecycle, SDLC = Software Development Lifecycle
- **CIA**: Confidentiality, Integrity, Availability (not Central Intelligence Agency)
- **DFD**: Data Flow Diagram (threat modeling artifact)
- **PSIRT**: Product Security Incident Response Team
- **SAST vs DAST**: Static Application Security Testing vs Dynamic Application Security Testing

### **PHASE TRANSITION TRIGGERS**

|**Phase**|**Entry Criteria**|**Exit Criteria**|
|---|---|---|
|**A1→A2**|Requirements gathered|Threat profile established|
|**A2→A3**|Architecture defined|Risk mitigation plan approved|
|**A3→A4**|Test plans created|Design security review complete|
|**A4→A5**|Testing executed|Remediation complete|
|**A5→PRS**|Final reviews passed|Product shipped|

### **EXAM SUCCESS STRATEGY**

**Pay attention to:**

- **Phase context** - Same activity name, different phase purposes
- **Verb tenses** - Planning vs executing vs reviewing
- **Scope indicators** - Initial, updated, final
- **Role-specific responsibilities** - Who does what
- **Sequential dependencies** - What must happen before/after