---
certifications:
- SOC 2 Type II
- ISO/IEC 27001:2013
- SOC 3
description: ''
kind: trust-center
layout: security
name: Trisotech Trust Center
name_suffix: Trust Center
overview: Trisotech maintains a public trust center documenting SOC 2 Type II, ISO/IEC 27001:2013, and SOC 3 compliance.
provider_name: Trisotech
provider_slug: trisotech
slug: trisotech-trust-center
source_filename: trisotech-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-09-02'\nmethod: searched\nsource: https://www.trisotech.com/security/\nurl: https://www.trisotech.com/security/\nname: Trisotech Cloud security and compliance page\nsummary: >-\n  Trisotech publishes a single security page rather than a trust centre. It names one\n  certification the company itself holds (SOC 2 Type II) and two it inherits from its hosting\n  provider (ISO/IEC 27001:2013 and SOC 3, both Google Cloud), states data residency in\n  Quebec, and describes its authentication and encryption posture. No report is downloadable\n  and there is no NDA-gated document portal.\ncertifications:\n- name: SOC 2 Type II\n  scope: Trisotech Cloud\n  held_by: Trisotech\n  framework: AICPA SSAE 18 / SOC for Service Organizations\n  statement: >-\n    \"achieved SOC 2 Type II compliance in accordance with American Institute of Certified\n    Public Accountants (AICPA) standards for SOC for Service Organizations also known as\n    SSAE 18\"\n  report_available: false\n\
  \  self_attested: true\n- name: ISO/IEC 27001:2013\n  scope: Data center\n  held_by: Google Cloud (hosting provider)\n  statement: >-\n    \"Trisotech guarantees that its data center provider complies with the ISO 27001:2013 norm\"\n  report_available: via the Google Cloud compliance portal\n  note: Inherited, not a certification of Trisotech itself.\n- name: SOC 3\n  scope: Data center\n  held_by: Google Cloud (hosting provider)\n  report_available: via the Google Cloud compliance portal\n  note: Inherited, not a certification of Trisotech itself.\ndata_residency:\n  region: Quebec, Canada\n  cloud: Google Cloud\n  legal_basis:\n    - Canadian federal privacy law\n    - Quebec provincial privacy act\nsecurity_posture_claims:\n  - Encryption in transit via SSL/HTTPS for all customer communications\n  - One-way hashed password storage\n  - SAML 2.0 and OpenID Connect authentication for user sign-in\nrelated_documentation:\n  - name: Secure Configuration Guide\n    url: https://cloud.trisotech.com/help/admin/secure-configuration-guide.html\n\
  \  - name: Administration security settings\n    url: https://cloud.trisotech.com/help/admin/security.html\nnot_claimed:\n  - HIPAA Business Associate Agreement\n  - FedRAMP\n  - PCI DSS\n  - ISO 27001 held by Trisotech itself\n  - ISO 27017 / 27018 / 27701\n  - Downloadable audit reports or a subprocessor list\nnote_on_healthcare: >-\n  Trisotech sells a Healthcare Feature Set with CDS Hooks and SMART on FHIR endpoints, but the\n  security page does not mention HIPAA, a BAA, or PHI handling. That is a notable gap for a\n  buyer in that market and is recorded here as an absence, not as a failure.\nevidence:\n- url: https://www.trisotech.com/security/\n  status: 200\n- url: https://cloud.trisotech.com/help/admin/secure-configuration-guide.html\n  status: 200\n- url: https://cloud.trisotech.com/help/admin/security.html\n  status: 200\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/trisotech/refs/heads/main/security/trisotech-trust-center.yml
summary_line: SOC 2 Type II, ISO/IEC 27001:2013, SOC 3
tags:
- Business Process Management
- Decision Management
- Workflow Automation
- Low Code
- BPMN
- DMN
- CMMN
- Healthcare
- FHIR
- Clinical Decision Support
- Standards
- AI Agents
- Model Context Protocol
- Enterprise Architecture
trust_url: https://www.trisotech.com/security/
---
