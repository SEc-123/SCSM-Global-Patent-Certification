
## 1.Governance Principles

To build a **decentralized**, **cross-national**, **cross-enterprise**, and **cross-government** system for **mutual recognition and intelligence sharing** in structured security investigation, the **knowledge write-back mechanism** is only enabled for entities that have successfully obtained **Organization-Level Certification**.  
This requirement ensures **data consistency**, **structural alignment**, and prevents **semantic fragmentation or confusion**.

Semantic knowledge sharing and validation must rely on a **unified semantic structure and behavior chain model**, which only certified Organization-Level entities are capable of fully supporting.

- **Node-Level products** (e.g., firewalls, EDRs) are responsible for **data collection or alert generation**;
- **Platform-Level products** (e.g., SIEM, SOAR) are responsible for **data aggregation and preliminary analysis**, but **must support features essential for Organization-Level Certification**, including:
  - Integration interfaces for AI-SIA Alliance,
  - Micro-model service endpoints,
  - Structured security investigation report generation.

Only **Organization-Level Certified entities** can establish the full semantic loop:

> `Field Normalization Layer（Node-Level Certification） → Behavior Chain Modeling Layer、AI Semantic Reasoning Layer、Micro-Scoring Layer（Platform-Level Certification） → Expert Feedback & Knowledge Loop（Organization-Level Certification）`

### Therefore:

- **Entities without Organization-Level Certification**, even if partially deploying certified products, **cannot participate in alliance-level semantic validation or knowledge reasoning**.
- **Uncertified Node or Platform-Level products** may cause **semantic incompatibility**, breaking the behavior chain structure.  
  Hence, **Node-Level and Platform-Level certification is a mandatory prerequisite**.

---

## 2.Clarification of Key Concepts

- The **Behavior Fragment Editor** and the **Knowledge Write-Back Mechanism** are two distinct concepts:

  - A behavior fragment refers to a single observable event, such as a brute-force login attempt; it is edited by local security analysts using AI and expert judgment, stored locally by the organization, and becomes an independent asset within the enterprise’s behavior fragment repository.

For example:
Tag: Brute Force Event BF ⇒ 100 failed login attempts (BCP) + 1 successful login (BPP) + pivot strength + additional conditions (e.g., within 24 hours).
A behavior fragment can represent an attack event, a normal event, or an abnormal but non-malicious activity.
Organizations define and adjust the rules based on their specific context to determine how each fragment should be interpreted;
  - The **Knowledge Write-Back Mechanism** refers to a **structured submission** of a **sequence of related events** and their **semantic coordinates**, allowing the alliance to:
    - Perform cross-organizational comparison,
    - Validate global patterns,
    - Evolve the shared knowledge base.

**The AI-SIA Alliance will annually publish a list of top-contributing enterprises and governments, recognizing their contributions and commitment to advancing global security investigation capabilities.**


## 3.1 SCSM License Usage Instructions

The patent owner grants the following usage rights for the Semantic Chain Security Model (SCSM) and all related patented concepts, methods, and structural definitions, subject to the terms outlined in this statement:

Permitted Standardization Citation

Standardization bodies and their working groups may cite the SCSM definition, terminology, and structure without additional authorization under FRAND (Fair, Reasonable, and Non-Discriminatory) principles, provided that the cited content remains identical to the original definition and is clearly attributed to the patent owner.

Any modification, redefinition, restructuring, or extension of the SCSM definition, terminology, or structure for inclusion in a standard requires prior written authorization from the patent owner.

Permitted Academic and Research Use

Academic publications, research reports, and educational materials may reference the SCSM theoretical framework and terminology without authorization, provided that such usage does not involve system implementation, functional deployment, or commercial exploitation.

Any experimental implementation, simulation, or functional testing—whether for commercial or non-commercial purposes—requires prior registration with the inventor of scsm and written authorization from the patent owner.

All such references must include proper attribution to the original source, clearly identifying the model name (SCSM) and citing the inventor or official publication as applicable.

Permitted Commercial Implementation

Any implementation, integration, or deployment of SCSM for commercial purposes—including but not limited to security products, platforms, and enterprise/government systems—requires an implementation license in accordance with Section 3.2 of this statement.

License categories include Node-Level, Platform-Level, and Organization-Level, each subject to their respective certification requirements.

Prohibited Uses Without Authorization

No party may modify, rebrand, or partially implement the SCSM framework in a manner intended to circumvent its structural or conceptual protection.

Unauthorized deployment, integration, or derivation—whether direct or indirect—constitutes patent infringement and will be subject to legal enforcement.

## 3.2 Implementation License (FRAND)

All implementation, integration, and deployment of this method must be made available to all qualified applicants under the principles of **Fair, Reasonable, Non-Discriminatory, and Transparent (FRAND-T)** licensing, and must comply with the corresponding certification requirements.  
Commercial implementation licenses are divided into **Node-Level / Platform-Level / Organization-Level** categories, in strict alignment with the Global Security Investigation Capability Certification Framework.

---

### 3.2.1 Node-Level Implementation License (Node-Level License ↔ Node-Level Certification)

**Fee Structure**: Annual license fee.  
**Eligible Applicants**: Security product / device vendors (e.g., Firewalls, WAF, Routers, EDR, HIDS, HDLP, IDS, IPS, NDLP, etc.).  
**Licensed Capabilities**:  
- Output data in compliance with the unified SCSM semantics and structured fields (including standardized time format, role entity labeling, etc.) to produce behavior fragments consumable by a licensed Platform-Level system;  
- Qualified products may apply for the **"SCSM-Compatible Behavior Node"** designation.
### Certification Rationale & Necessity

Security products from different vendors and categories often use inconsistent **data formats**, **field naming conventions**, and **semantic structures**.  
Examples include:  
- Time formats vary (UNIX timestamp, 24-hour clock, 12-hour clock, differing time zones).  
- Role or subject identifiers differ (`hostip`, `ip`, `srcip`, etc.).  
- Perimeter devices often lack a **Triple-Mapping Mechanism** for correlating roles, behaviors, and tags.  

This certification ensures that all node-level devices provide a **unified semantic interface** aligned with the **SCSM Security Investigation Language**, **with unified and unambiguous subject(Srcip) identifiers**.

It standardizes field alignment and semantic tagging across heterogeneous products, enabling **seamless integration** within platform-level systems.  

By implementing these requirements, products from different vendors and categories can provide standardized transformation interfaces to platform-level products within a unified and interoperable investigation framework, thereby ensuring consistent interpretation, processing, and correlation of behavioral data at the platform level.

 -**Node-Level Certification Requirements (Product Specifications)**:  
1.  -**Unified Interfaces and Configuration**:  
   - Provide a data output interface and a configurable management interface for selecting output fields;  
   - Maintain unified role identifiers and a standardized time format (YYYY-MM-DD, hh:mm:ss, time zone consistent).  
 -**Node-level certification ensures standardized input structures, while organization-level structured investigation certification ensures standardized output and international knowledge sharing. Without  certification, unstructured data from uncertified systems may contaminate the interoperability and trustworthiness of investigations.**
 
**Perimeter Devices** (e.g., WAF, Routers, Firewalls):  
   - Must support a **Triple-Mapping Mechanism** (Role–Behavior–Tag mapping).  
3. **Host Devices** (e.g., EDR, HIDS, HDLP):  
   - `hostip` must be mapped to `srcip`;  
   - Must include the capability to semantically interpret security logs, system logs, and application logs.  
4. **Network Devices** (e.g., IDS, IPS, NDLP):  
   - Output must comply with SCSM semantic field specifications, support behavior fragment processing, and include structured tagging.

---

### 3.2.2 Platform-Level Implementation License (Platform-Level License ↔ Platform-Level Certification)

**Fee Structure**: Annual license fee.  
**Eligible Applicants**: Log aggregation / correlation platforms, SIEM/SOAR systems, next-generation SOC platforms (including MSSP / SaaS models).  
**Licensed Capabilities**:  
- Ingest data from licensed Node-Level sources and maintain semantic integrity throughout the processing pipeline;  
- Construct valid semantic behavior chains, with capabilities including behavior indexing, pivot tracking, semantic timelines, and modular structured investigation tools;  
- Provide structured investigation capabilities to multiple tenants or external customers (platform-as-a-service model).
### Platform-Level Certification Necessity

The necessity for platform-level certification recommends adopting a next-generation SOC paradigm security operations platform.  
Through deployment integrated with node-level facilities, unified and standardized logs are collected into the **EBD** (Event Behavior Database).  

In this paradigm, **SIEM is no longer just a log collector**, but, through certified modular integration, enables:  
- AI-driven investigation and reasoning;  
- Local editing and customization of behavior fragments;  
- Integration with the **AI-SIA Alliance** knowledge-sharing mechanism;  
- Structured platform support for **organization-level certification** of security structured investigation capabilities;  
- Generation of structured security investigation reports.  

**Note**: 
1.Any SOC platform (including SaaS, cloud-based SOC, or MSSP model) falls under the Platform-Level License category.
2.Due to the structural and technological neutrality as well as the open-source adaptability of SCSM, enterprises and governments may independently develop SOC platforms in accordance with the platform-level standards. However, such SOC platforms must still obtain separate platform-level certification, since only a platform certified at this level qualifies as the semantic engine for security investigation.

**Platform-Level Certification Requirements (Next-Generation SOC Paradigm)**:  
1. **Role Database & Interaction**:  
   - Integrate a role database with a chat window and retain security investigation chat history.  
2. **Concurrent Visualization & Investigation Results**:  
   - Display database-driven visualization results on one panel, and investigation results on another;  
   - Each log entry is linked to AI reasoning evidence via `logid`, can be saved as a "Confirmed Attack Event", and output as a structured security report.  
3. **Structured Investigation Report Output**:  
   - Must support exporting structured security investigation reports in SCSM format.  
4. **Knowledge Base Functionality**:  
   - Include a behavior fragment structured knowledge base, with the ability to add micro-model explanation functions.  
5. **Threat Intelligence Interoperability**:  
   - Integrate with AI-SIA Alliance exclusive threat intelligence capabilities, enabling retrieval of alliance attack chains (composed of behavior fragments);  
   - Provide a knowledge write-back interface for alliance sharing.  
6. **Micro-Model Integration Service Interface**:  
   - Support dynamic addition/removal of micro-models;  
   - Support local AI model integration .  
7. **Statistics & Visualization**:  
   - Provide interfaces for role statistics, behavior statistics, behavior classification, and behavior chain visualization.  
8. **Tagging & Knowledge Write-Back Mechanism**:  
   - BFL (BCP, BPP) tags are generated by AI reasoning; experts may validate, adjust, and write back to the knowledge base (e.g., brute force attack recognition and condition definition).  
9. **Micro-Model Classification**:  
   - **Private Models**: Built, trained, and tested internally by the licensee;  
   - **Alliance Common Models**: Provided by the alliance for cross-domain model training and service (e.g., analyzing external IP connection time and geolocation for perimeter devices).

---

### 3.2.3 Organization-Level Implementation License (Organization-Level License ↔ Organization-Level Certification)

**Fee Structure**: Annual license fee for enterprises; one-time license fee for governments and critical information infrastructure.  
**Eligible Applicants**: Enterprises, governments, and critical information infrastructure end-users. 
### Organization-Level Certification Necessity

The necessity for organization-level certification is that enterprises or governments, by deploying node-level and platform-level licensed products and devices, establish structured security investigation capabilities and apply for **organization-level security investigation capability certification**.  
Becoming a member of the **AI-SIA Alliance**(a closed‑loop design of identity id‑service‑data) enables cross-country and cross-system access to the alliance’s exclusive **Behavior Chain Shared Knowledge Base (BC‑KB) Platform** and **Micro‑model Inference‑as‑a‑Service(IaaS)** (normally subject to fees), ensuring:  
- Long-term retention of security investigation capabilities;  
- Access to the latest security investigation intelligence from different regions;  
- The ability to investigate whether similar attacks exist locally.  
 
**Licensed Capabilities**:  
- Establish complete structured investigation capability within the organization: deploy Node-Level licensed devices; operate a Platform-Level licensed system to generate behavior chains;  
- Employ Node-Level and Platform-Level products certified by the AI-SIA Alliance, and demonstrate the capability to produce structured security investigation reports in compliance with the semantic investigation framework.;  
- Operate with bi-directional integration into the SCSM knowledge write-back mechanism.

**Special Provisions**:  
- Initial Organization-Level licensing includes all capabilities except "knowledge write-back", which must be implemented via the AI-SIA Alliance;  
- Behavior fragments are locally generated and stored by the SOC platform within the enterprise or government;  
- In the initial phase, Organization-Level licensing does not mandate the use of Node-Level and Platform-Level products; certification will be required as the alliance evolves.
- The rationale for requiring governments to obtain structured security investigation capability certification at the organization level is straightforward: governments also need to connect to the globally interconnected shared knowledge base for read and write-back mechanisms. Without first demonstrating their structured investigation capability, they risk contaminating interoperability and trustworthiness of investigations with non-structured data.
---
**Special Friendly Provisions for Government-Level Licensing in Developing Countries**: 
- For small-state governments in developing countries, the following special mechanism shall be available to Apply for Patent Fee Reduction or Free Licensing:
Eligible governments may submit a formal request to the Expert Committee. Upon preliminary approval, the committee shall forward the application to the Alliance Licensing Office. The final decision on fee reduction or waiver rests with the inventor.

### General FRAND Constraints (Applicable to All Three License Levels)

1. **Fees & Conditions**: Uniform for all qualified applicants within the same license level, with full pricing transparency; no quotas, no implicit discriminatory terms.  
2. **Sub-Licensing**: Sub-licensing to third parties is prohibited; Node-Level and Platform-Level licenses may be embedded into security products for external distribution.  
3. **Compliance Audit**: The patent holder may conduct compliance audits within the scope of the license.  
4. **Infringement Notice**: Any implementation, integration, or deployment without written authorization constitutes infringement; substitution of terminology, minor logical modifications, or derivative restructuring without the inventor’s authorization likewise constitutes infringement.
