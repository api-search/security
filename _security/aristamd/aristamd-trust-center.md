---
api_specs:
- filename: aristamd-comments-api-openapi.yml
  format: yaml
  label: AristaMD Comments API
  slug: aristamd-comments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aristamd/refs/heads/main/openapi/aristamd-comments-api-openapi.yml
- filename: aristamd-diagnostic-api-openapi.yml
  format: yaml
  label: AristaMD Diagnostic API
  slug: aristamd-diagnostic-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aristamd/refs/heads/main/openapi/aristamd-diagnostic-api-openapi.yml
- filename: aristamd-econsults-api-openapi.yml
  format: yaml
  label: AristaMD E Consults API
  slug: aristamd-econsults-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aristamd/refs/heads/main/openapi/aristamd-econsults-api-openapi.yml
- filename: aristamd-intergy-patients-api-openapi.yml
  format: yaml
  label: AristaMD Intergy/Patients API
  slug: aristamd-intergy-patients-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aristamd/refs/heads/main/openapi/aristamd-intergy-patients-api-openapi.yml
- filename: aristamd-panelists-api-openapi.yml
  format: yaml
  label: AristaMD Panelists API
  slug: aristamd-panelists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aristamd/refs/heads/main/openapi/aristamd-panelists-api-openapi.yml
- filename: aristamd-patients-api-openapi.yml
  format: yaml
  label: AristaMD Patients API
  slug: aristamd-patients-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aristamd/refs/heads/main/openapi/aristamd-patients-api-openapi.yml
- filename: aristamd-requests-api-openapi.yml
  format: yaml
  label: AristaMD Requests API
  slug: aristamd-requests-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aristamd/refs/heads/main/openapi/aristamd-requests-api-openapi.yml
- filename: aristamd-reviews-api-openapi.yml
  format: yaml
  label: AristaMD Reviews API
  slug: aristamd-reviews-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aristamd/refs/heads/main/openapi/aristamd-reviews-api-openapi.yml
- filename: aristamd-specialties-api-openapi.yml
  format: yaml
  label: AristaMD Specialties API
  slug: aristamd-specialties-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aristamd/refs/heads/main/openapi/aristamd-specialties-api-openapi.yml
- filename: aristamd-specialty-api-openapi.yml
  format: yaml
  label: AristaMD Specialty API
  slug: aristamd-specialty-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aristamd/refs/heads/main/openapi/aristamd-specialty-api-openapi.yml
- filename: aristamd-users-api-openapi.yml
  format: yaml
  label: AristaMD Users API
  slug: aristamd-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aristamd/refs/heads/main/openapi/aristamd-users-api-openapi.yml
- filename: aristamd-workup-checklists-api-openapi.yml
  format: yaml
  label: AristaMD Workup Checklists API
  slug: aristamd-workup-checklists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aristamd/refs/heads/main/openapi/aristamd-workup-checklists-api-openapi.yml
certifications:
- SOC 2
description: ''
kind: trust-center
layout: security
name: Aristamd Trust Center
name_suffix: Trust Center
overview: AristaMD maintains a public trust center documenting SOC 2 compliance.
provider_name: AristaMD
provider_slug: aristamd
slug: aristamd-trust-center
source_filename: aristamd-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-06'\nmethod: searched\nprobe: true\nurl: https://www.aristamd.com/security/\nsource: https://www.aristamd.com/security/\nstatus: 200\nnote: >-\n  The automated probe (probe-security-programs.py) reported trust=none because it\n  looks for trust.<domain> / security.<domain> subdomains and a /trust or\n  /compliance path, none of which exist. AristaMD does publish a substantive\n  security posture page at /security/ on the marketing host; this artifact was\n  written by hand from that page after the probe missed it.\n\ncertifications:\n# Recorded exactly as AristaMD states them. AristaMD describes SOC 2 as the\n# FRAMEWORK its Information Security Program follows and cites independent\n# third-party assessments — it does not publish an attestation report, a\n# certificate, a report date or a named auditor on the public page. That\n# distinction is preserved here rather than flattened into \"SOC 2 certified\".\n- name: SOC 2\n  claim_type: framework-followed\n\
  \  attestation_published: false\n  verbatim: >-\n    \"Our Information Security Program follows the criteria set forth by the SOC 2\n    Framework. SOC 2 is a widely known information security auditing procedure\n    created by the American Institute of Certified Public Accountants.\"\n\nprogram:\n  organizational:\n  - Information Security Program communicated throughout the organization\n  - Independent third-party assessments of security and compliance controls\n  - Independent third-party penetration testing performed at least annually\n  - Defined and documented roles and responsibilities; policies reviewed and accepted by staff\n  - Security awareness training covering phishing and password management\n  - Industry-standard confidentiality agreements signed before first day\n  - Background checks on all new team members\n  cloud:\n  - Hosted on a combination of Amazon Web Services and Google Cloud Platform\n  - All data hosted in databases located in the United States\n  - Encryption\
  \ at rest for all databases\n  - Encryption in transit — TLS/SSL only\n  - Vulnerability scanning and active threat monitoring\n  - Logging and monitoring of cloud services\n  - Backup via the hosting provider; monitoring alerts on failures\n  - Documented incident response with escalation, rapid mitigation and communication\n  access:\n  - Access to cloud infrastructure limited to authorized employees by role\n  - Principle of least privilege for identity and access management\n  - Quarterly access reviews for all staff with access to sensitive systems\n  - Minimum password complexity requirements\n  - Company-issued laptops use a password manager\n  vendor_and_risk:\n  - Vendor risk determined and reviewed before authorizing a new vendor\n  - At least annual risk assessments, including fraud considerations\n\ncontact:\n  security: info@aristamd.com\n  verbatim: >-\n    \"If you have any questions, comments or concerns or if you wish to report a\n    potential security issue, please contact\
  \ info@aristamd.com\"\n  legal_address: AristaMD, Inc., Attn Legal, 4660 La Jolla Village Dr., Suite 100\n    #1535, San Diego\n\nnot_published:\n# Recorded because a healthcare buyer's security review will ask for each of these.\n- SOC 2 Type II report or bridge letter (not linked, not gated behind a form)\n- Name of the auditor or assessment firm\n- Date or period of the most recent assessment\n- HIPAA statement or BAA availability — notable, since the platform handles US PHI\n- ISO 27001, HITRUST, PCI DSS or FedRAMP\n- Subprocessor list\n- Automated trust portal (Vanta/Drata/SafeBase style)\n- security.txt (RFC 9116) at any host\n- Bug bounty or coordinated disclosure program\n\nevidence:\n- source: https://www.aristamd.com/security/\n  status: 200\n  keywords: [information security program, soc 2, third-party audits, penetration\n    testing, encryption at rest, encryption in transit, incident response, least\n    privilege, risk assessments, vendor risk]\n- source: https://trust.aristamd.com/\n\
  \  status: not-resolved\n- source: https://www.aristamd.com/trust/\n  status: 404\n- source: https://www.aristamd.com/compliance/\n  status: 404\n- source: https://www.aristamd.com/hipaa/\n  status: 404\n\nx-evidence:\n  fetched: '2026-08-06'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aristamd/refs/heads/main/security/aristamd-trust-center.yml
summary_line: SOC 2
tags:
- Company
- Healthcare
- Digital Health
- Telehealth
- eConsult
- Specialty Care
- Referrals
- Care Coordination
- Health Plans
- Medicaid
- HL7
- Electronic Health Records
trust_url: https://www.aristamd.com/security/
---
