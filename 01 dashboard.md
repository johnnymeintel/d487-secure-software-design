# 🛡️ WGU D487 Secure Software Design - Complete Exam Guide

## 📊 Dashboard

### 🎯 Quick Navigation

- [🎯 Course Overview](#-course-overview) - Core competencies and exam focus
- [📚 Key Frameworks & Models](#-key-frameworks--models) - BSIMM, STRIDE, DREAD, PASTA
- [🔍 Security Testing](#-security-testing) - Testing types and methodologies
- [⚙️ SDL Integration](#️-sdl-integration) - Agile security and requirement types
- [🔐 Core Security Principles](#-core-security-principles) - Access control and data protection
- [🚨 Common Vulnerabilities](#-common-vulnerabilities) - Attack types and countermeasures
- [📋 Exam Question Types](#-exam-question-types) - What to expect on the exam
- [⚠️ Critical Exam Tips](#️-critical-exam-tips) - Things to watch out for
- [📅 3-Day Study Timeline](#-3-day-study-timeline) - Your preparation schedule
- [📖 Essential Terminology](#-essential-terminology) - Key terms and definitions

---

## 🎯 Course Overview

### Core Competencies

- **4029.2.1**: Security principles, standards, and methods within SDLC
- **4029.2.2**: Software requirements and risk assessment for threat mitigation
- **4029.2.3**: Security test plan documentation and implementation strategies
- **4029.2.4**: Software testing and deployment effectiveness for security/privacy

### Exam Distribution (66 questions)

- 🎭 **Threat Modeling & Risk Assessment** (35% - ~21 questions)
- 🔄 **SDL Integration & Security Gates** (25% - ~15 questions)
- 💻 **Secure Coding & Vulnerabilities** (20% - ~12 questions)
- 🧪 **Security Testing Methodologies** (15% - ~9 questions)
- 📋 **Standards & Post-Release** (5% - ~3 questions)

---

## 📚 Key Frameworks & Models

### 🏗️ BSIMM (Building Security In Maturity Model)

**Purpose**: Studies real-world software security initiatives for benchmarking

**Four Domains**:

- 🏛️ **Governance**: Strategy, compliance, training programs
- 🧠 **Intelligence**: Attack models, security features, standards research
- 🔨 **SSDL Touchpoints**: Hands-on security activities (code review, testing)
- 🚀 **Deployment**: Configuration management, vulnerability management

**Key Distinction**: BSIMM is **descriptive** (what organizations actually do) vs SAMM is **prescriptive** (what you should do)

### ⚔️ STRIDE Threat Modeling

- **S**poofing: Identity impersonation attacks
- **T**ampering: Unauthorized data modification
- **R**epudiation: Denial of performed actions
- **I**nformation Disclosure: Unauthorized data access
- **D**enial of Service: Service availability attacks
- **E**levation of Privilege: Unauthorized access escalation

**Application Methods**:

- 🔍 **STRIDE-per-element**: Analyze each individual component/object
- ⚙️ **STRIDE-per-process**: Focus only on processes
- 🌉 **STRIDE-per-trust-boundary**: Analyze security boundary crossings
- 🔄 **STRIDE-per-interaction**: Focus on data flows between components

### 💥 DREAD Risk Scoring

**Ternary Scale**: High=3, Medium=2, Low=1

- **D**amage: Potential impact severity
- **R**eproducibility: How easily attack can be repeated
- **E**xploitability: Difficulty of executing the attack
- **A**ffected users: Scope and number of impacted users
- **D**iscoverability: How easy vulnerability is to find

**Total Score Interpretation**:

- 13-15 points = High Risk
- 8-12 points = Medium Risk
- 5-7 points = Low Risk

### 🔬 PASTA (Process for Attack Simulation and Threat Analysis)

**Seven-Stage Methodology**:

1. **Define Objectives** - Business and security requirements
2. **Define Technical Scope** - Application boundaries and components
3. **Application Decomposition** - Break down architecture and data flows
4. **Threat Analysis** - Identify potential threats and attack vectors
5. **Vulnerability and Weakness Analysis** - **Design flaw analysis occurs here**
6. **Attack Modeling** - Develop specific attack scenarios
7. **Risk and Impact Analysis** - Evaluate business impact and likelihood

### 🏗️ Microsoft Threat Modeling

**Four-Step Process**:

1. **Diagram** - Create data flow diagrams
2. **Identify** - Find threats using STRIDE
3. **Mitigate** - Apply countermeasures
4. **Validate** - Verify threat mitigation effectiveness

### 🏢 OCTAVE (Operationally Critical Threat, Asset, and Vulnerability Evaluation)

**Three Phases**:

- **Phase 1**: Build asset-based threat profiles
- **Phase 2**: Identify infrastructure vulnerabilities
- **Phase 3**: Develop security strategy and plans

### 🎯 TRIKE

**Risk-based approach**:

- **Requirements Model** - Define security requirements
- **Implementation Model** - Analyze system implementation
- **Risk Model** - Calculate risk levels for threats


### 📚 SDL Phases

- **SDL A1:** Security Assessment (Discovery Phase)
	- Identify product risk profile (security changes needed to cater to different markets)
	- SDL project outline (map SDL to dev schedule)
	- Applicable laws and regulations
	- Accuracy of the threat profile (customers misuse and change things)
	- Certification requirements
	- List of third-party software
	- Metric template
	- Privacy Impact Assessment plan
		- Summary of the Legislation
		- Required Process Steps
		- Technologies and Techniques
		- Additional Resources
- **SDL A2:** Architecture
	- Identification of business requirements and risk
	- Data Flow Diagram
	- Threat modeling via STRIDE / DREAD / risk = likelihood x impact
		- Identify security objectives
		- Survey the application
		- Decompose it
		- Identify threats
		- Identify vulnerabilities 
	- Risk mitigation
	- Policy compliance analysis
- **SDLA3:** Design and Development 
	- Analysis of policy compliance (review)
	- Create the test plan documentation
	- Static analysis
	- Update your threat model
	- Design security analysis and review
	- Privacy implementation assessment 
	- 1974 UVA Saltzer/Schroeder
- **SDLA4:** Design and Development (readiness)
	- Policy compliance analysis
	- Security test case execution
	- Static analysis
	- Dynamic analysis
	- Fuzz testing
	- Manual code review
	- Privacy validation and remediation
- **SDLA5:** Ship
	- Final security review
	- Vulnerability scan
	- Penetration testing
	- Open source licensing review
	- Final security review
	- Final privacy review
	- Customer engagement framework
- **PRSA1:** External Vulnerability Disclosure Response
- **PRSA2:** Third-Party Reviews
- **PRSA3:** Post-Release Certifications
- **PRSA4:** Internal Review for New product Combinations or Cloud Deployments
- **PRSA5:** Security Architectural Reviews and Tool-Based Assessments of Current, Legacy, and M&A Products and Solutions
	- External vulnerability disclosure response process
	- Post-release certifications
	- Third-party security reviews
	- Security strategy and process for legacy code, M&A, and EOL plans

---

## 🔍 Security Testing

### 📊 Analysis Methods

|Method|Description|When to Use|
|---|---|---|
|🔍 **Static Analysis**|Code examination without execution|Early development, code review|
|▶️ **Dynamic Analysis**|Testing while program executes|Runtime behavior, integration testing|
|📖 **White-box**|Full access to source code/docs|Comprehensive internal testing|
|🔘 **Gray-box**|Limited internal knowledge|Hybrid approach|
|⚫ **Black-box**|External perspective only|User experience testing|

### 🧪 Testing Categories

- 🎯 **Functional Testing**: Validates application requirements compliance
- 🔧 **Unit Testing**: Individual component testing
- 🔗 **Integration Testing**: Component interaction testing
- 🔄 **Regression Testing**: Ensures changes don't break existing functionality

### 🛠️ Security Testing Tools

- **SonarQube**: Static code analysis (SAST)
- **OWASP ZAP**: Dynamic application security testing (DAST)
- **Burp Suite**: Web application security testing

---

## ⚙️ SDL Integration

### 🏃‍♂️ Agile Security Requirement Types

- 🔄 **Every-sprint Requirements**: Applied continuously (input validation, authentication)
- 🪣 **Bucket Requirements**: Triggered by specific technologies (RPC fuzz testing)
- 1️⃣ **One-time Requirements**: Implemented once per project (initial architecture)
- ✅ **Final Security Review Requirements**: Pre-release validation activities

### 📋 Key SDL Deliverables

- 📅 **SDL Project Outline**: Security milestones integrated with development schedule
- ✅ **Policy Compliance Analysis**: Verification of adherence to organizational security rules
- 🗂️ **Threat Modeling Artifacts**: Updated documentation with newly identified vulnerabilities
- 🏢 **Security Strategy for M&A**: Framework for integrating acquired products

### 🚪 Security Gates & Reviews

- **Final Security Review Outcomes**:
    - ✅ **Passed**: All issues resolved, all requirements met
    - ⚠️ **Passed with exceptions**: Minor acceptable risks remain
    - ❌ **Not passed (escalation)**: Critical issues require escalation
    - ⏸️ **Not passed (no escalation)**: Issues exist but not critical

---

## 🔐 Core Security Principles

### 🛡️ Access Control Principles

- 🔒 **Principle of Least Privilege**: Users get minimum necessary access
- 👥 **Role-Based Access Control (RBAC)**: Access based on user roles
- 🤝 **Separation of Duties**: Multiple people required for critical tasks
- 🏰 **Defense in Depth**: Multiple layers of protection

### 🛡️ Data Protection

- ✅ **Input Validation**: Verify user input meets expected criteria (type, size, range)
- 🔤 **Output Encoding**: Prevent XSS by encoding special characters (<, >, ", ', &)
- 💉 **Parameterized Queries**: Prevent SQL injection by separating code from data
- 🔐 **Cryptographic Practices**: Use proven algorithms (AES, RSA, SHA-256)

### ⚙️ Configuration Security

- 🔧 **System Configuration**: Maintain latest approved versions of all components
- 👤 **Default Account Management**: Disable/remove default credentials immediately
- 🌐 **Communication Security**: Encrypt all data in transit (TLS/SSL)

---

## 🚨 Common Vulnerabilities

### 💉 Injection Attacks

|Vulnerability|Countermeasure|Implementation|
|---|---|---|
|SQL Injection|Parameterized Queries|Use placeholders, not string concatenation|
|XSS|Output Encoding|Encode <, >, ", ', & characters|
|File Upload|Input Validation|Validate file type, size, content|

### 🔑 Authentication & Session Issues

- 🔒 **Weak Passwords**: Enforce complexity (8+ chars, upper, number, special)
- ⏰ **Session Management**: Proper timeouts and session handling
- ⬆️ **Privilege Escalation**: Restore proper privileges after exceptions

### 🔐 Cryptographic Failures

- 🧂 **Weak Hashing**: Use strong, salted hashing (bcrypt, Argon2, scrypt)
- ⚙️ **Default Configurations**: Change all default settings and credentials
- 🔑 **Key Management**: Proper encryption key storage and rotation

---

## 📋 Exam Question Types

### 🎭 Scenario-Based Questions (40%)

**Example Pattern**: "A security team discovered..." or "During testing, an analyst found..."

- Real-world application of security concepts
- SDL phase identification and appropriate activities
- Vulnerability remediation strategies

### 📖 Definition & Classification (25%)

**Example Pattern**: "Which framework studies real-world security initiatives?"

- Framework purposes and distinctions
- Requirement type classifications
- Security principle definitions

### 🔧 Technical Implementation (20%)

**Example Pattern**: "How should existing security controls be adjusted?"

- Specific countermeasures for vulnerabilities
- Secure coding practice implementation
- Configuration and remediation steps

### 🔄 Process & Workflow (15%)

**Example Pattern**: "What is the next step in the process?"

- PSIRT workflow sequences
- SDL phase activities
- Incident response procedures

---

## ⚠️ Critical Exam Tips

### 🔍 Key Distinctions to Remember

- **BSIMM vs SAMM**: BSIMM studies what organizations do, SAMM prescribes what to do
- **Static vs Dynamic**: Static = no execution, Dynamic = while running
- **White vs Black box**: White = full internal access, Black = external perspective only
- **Every-sprint vs Bucket**: Every-sprint = always required, Bucket = when specific tech used
- **PASTA vs Microsoft**: PASTA has 7 stages, Microsoft has 4 steps (Diagram, Identify, Mitigate, Validate)
- **STRIDE applications**: Per-element (most granular), per-process (processes only), per-trust-boundary (boundaries), per-interaction (data flows)

### 🎯 Keyword Recognition

- "**Real-world initiatives**" → BSIMM
- "**Without executing**" → Static Analysis
- "**All traffic encrypted**" → Communication Security
- "**Default settings**" → Remove/disable default accounts
- "**Easily repeated**" → Reproducibility (DREAD)
- "**Design flaw analysis**" → PASTA Stage 5 (Vulnerability and Weakness Analysis)
- "**Data flow diagram**" → Microsoft Threat Modeling Step 1 (Diagram)
- "**Seven stages**" → PASTA methodology
- "**Four steps**" → Microsoft Threat Modeling

### 🚨 Common Traps

- Don't confuse **remediation** (how to fix) with **detection** (how to find)
- **Final Security Review** needs ALL issues resolved for "Passed" status
- **Bucket requirements** are triggered by technology, not always applied
- **PSIRT workflow**: Fix development comes before customer notification

---

## 📅 3-Day Study Timeline

### 📚 Day 1: Foundations & Frameworks


- [[#📚 Key Frameworks & Models]] - Focus on BSIMM, STRIDE, DREAD
- Create framework comparison chart
- Practice distinguishing BSIMM vs SAMM questions
- [[#⚙️ SDL Integration]] - Agile security requirements
- [[#🔐 Core Security Principles]] - Access control and data protection
- Practice scenario-based questions
- Review [[#📖 Essential Terminology]]
- Create flashcards for key terms

### 🔍 Day 2: Testing & Vulnerabilities


- [[#🔍 Security Testing]] - Testing types and methodologies
- [[#🚨 Common Vulnerabilities]] - Attack types and countermeasures
- Focus on static vs dynamic analysis distinctions
- Practice technical implementation questions
- Review vulnerability remediation strategies
- Create vulnerability → countermeasure mapping
- Review [[#⚠️ Critical Exam Tips]]
- Practice keyword recognition exercises

### ✅ Day 3: Integration & Practice


- Full practice exam simulation
- Identify weak areas from practice results
- Targeted review of weak areas
- Focus on [[#📋 Exam Question Types]] patterns
- Review process workflows (PSIRT, SDL phases)
- Final review of [[#⚠️ Critical Exam Tips]]
- Relaxation and preparation for exam day

---

## 📖 Essential Terminology

### 🏗️ Frameworks & Standards

- **BSIMM**: Building Security In Maturity Model - studies real-world practices
- **SAMM**: Software Assurance Maturity Model - prescriptive framework
- **STRIDE**: Threat modeling methodology (6 threat categories)
- **DREAD**: Risk scoring system (5 factors)
- **PASTA**: Process for Attack Simulation and Threat Analysis (7 stages)
- **Microsoft Threat Modeling**: 4-step process (Diagram, Identify, Mitigate, Validate)
- **OCTAVE**: Operationally Critical Threat, Asset, and Vulnerability Evaluation
- **TRIKE**: Risk-based threat modeling approach
- **ISO 27001**: Information Security Management Systems standard
- **CVE**: Common Vulnerabilities and Exposures naming system
- **OWASP**: Open Web Application Security Project

### 🔒 Security Concepts

- **SDL**: Security Development Lifecycle
- **SAST**: Static Application Security Testing
- **DAST**: Dynamic Application Security Testing
- **PSIRT**: Product Security Incident Response Team
- **XSS**: Cross-Site Scripting
- **CSRF**: Cross-Site Request Forgery
- **RBAC**: Role-Based Access Control
- **MFA**: Multi-Factor Authentication
- **TLS**: Transport Layer Security
- **AES**: Advanced Encryption Standard

### 🧪 Testing & Development

- **CI/CD**: Continuous Integration/Continuous Deployment
- **DevSecOps**: Development, Security, and Operations integration
- **RACI**: Responsible, Accountable, Consulted, Informed matrix
- **Threat Modeling**: Systematic threat identification process
- **Penetration Testing**: Simulated cyber attack testing
- **Vulnerability Assessment**: Security weakness identification
- **Code Review**: Source code security examination

### 🎯 Key Principles

- **Defense in Depth**: Multiple security layers strategy
- **Least Privilege**: Minimum necessary access principle
- **Fail Safe**: Secure failure mode principle
- **Zero Trust**: Never trust, always verify model
- **Separation of Duties**: Fraud prevention control
- **Input Validation**: User input verification process
- **Output Encoding**: XSS prevention technique
- **Parameterized Queries**: SQL injection prevention method

---

## 🎯 Final Success Tips

### 🧠 Mental Preparation

- Get adequate sleep before the exam
- Arrive early and settle in calmly
- Read questions carefully - watch for negative words

### 📝 Exam Strategy

- Eliminate obviously wrong answers first
- Look for keyword clues in questions
- Trust your first instinct on difficult questions
- Manage time effectively (1.5 minutes per question)

### 🔍 Question Analysis Approach

1. Identify what the question is really asking
2. Look for context clues and keywords
3. Apply the appropriate framework or principle
4. Choose the most specific and accurate answer

**Remember**: This exam tests practical application of security in real-world development scenarios. Focus on understanding WHY certain practices are recommended, not just memorizing definitions.

Good luck! 🍀
