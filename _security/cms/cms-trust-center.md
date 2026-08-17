---
api_specs:
- filename: cms-bcda-openapi.yml
  format: yaml
  label: CMS Beneficiary Claims Data API (BCDA)
  slug: cms-beneficiary-claims-data-api-bcda
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cms/refs/heads/main/openapi/cms-bcda-openapi.yml
- filename: cms-ab2d-openapi.yml
  format: yaml
  label: CMS AB2D API (Claims Data to Part D Sponsors)
  slug: cms-ab2d-api-claims-data-to-part-d-sponsors
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cms/refs/heads/main/openapi/cms-ab2d-openapi.yml
- filename: cms-api-reference-api-openapi.yml
  format: yaml
  label: Centers for Medicare and Medicaid Services API Reference API
  slug: cms-api-reference-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cms/refs/heads/main/openapi/cms-api-reference-api-openapi.yml
- filename: cms-bulk-data-api-openapi.yml
  format: yaml
  label: Centers for Medicare and Medicaid Services Bulk Data API
  slug: cms-bulk-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cms/refs/heads/main/openapi/cms-bulk-data-api-openapi.yml
- filename: cms-code-search-api-openapi.yml
  format: yaml
  label: Centers for Medicare and Medicaid Services Code Search API
  slug: cms-code-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cms/refs/heads/main/openapi/cms-code-search-api-openapi.yml
- filename: cms-cost-search-api-openapi.yml
  format: yaml
  label: Centers for Medicare and Medicaid Services Cost Search API
  slug: cms-cost-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cms/refs/heads/main/openapi/cms-cost-search-api-openapi.yml
- filename: cms-enrollments-api-openapi.yml
  format: yaml
  label: Centers for Medicare and Medicaid Services Enrollments API
  slug: cms-enrollments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cms/refs/heads/main/openapi/cms-enrollments-api-openapi.yml
- filename: cms-geography-api-openapi.yml
  format: yaml
  label: Centers for Medicare and Medicaid Services Geography API
  slug: cms-geography-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cms/refs/heads/main/openapi/cms-geography-api-openapi.yml
- filename: cms-households-eligibility-api-openapi.yml
  format: yaml
  label: Centers for Medicare and Medicaid Services Households & Eligibility API
  slug: cms-households-eligibility-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cms/refs/heads/main/openapi/cms-households-eligibility-api-openapi.yml
- filename: cms-insurance-issuers-api-openapi.yml
  format: yaml
  label: Centers for Medicare and Medicaid Services Insurance Issuers API
  slug: cms-insurance-issuers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cms/refs/heads/main/openapi/cms-insurance-issuers-api-openapi.yml
- filename: cms-insurance-plans-api-openapi.yml
  format: yaml
  label: Centers for Medicare and Medicaid Services Insurance Plans API
  slug: cms-insurance-plans-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cms/refs/heads/main/openapi/cms-insurance-plans-api-openapi.yml
- filename: cms-plans-api-openapi.yml
  format: yaml
  label: Centers for Medicare and Medicaid Services Plans API
  slug: cms-plans-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cms/refs/heads/main/openapi/cms-plans-api-openapi.yml
- filename: cms-provider-drug-coverage-api-openapi.yml
  format: yaml
  label: Centers for Medicare and Medicaid Services Provider & Drug Coverage API
  slug: cms-provider-drug-coverage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cms/refs/heads/main/openapi/cms-provider-drug-coverage-api-openapi.yml
- filename: cms-capability-api-openapi.yml
  format: yaml
  label: Centers for Medicare and Medicaid Services Capability API
  slug: centers-for-medicare-and-medicaid-services-capability-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cms/refs/heads/main/openapi/cms-capability-api-openapi.yml
- filename: cms-coverage-api-openapi.yml
  format: yaml
  label: Centers for Medicare and Medicaid Services Coverage API
  slug: centers-for-medicare-and-medicaid-services-coverage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cms/refs/heads/main/openapi/cms-coverage-api-openapi.yml
- filename: cms-explanationofbenefit-api-openapi.yml
  format: yaml
  label: Centers for Medicare and Medicaid Services ExplanationOfBenefit API
  slug: centers-for-medicare-and-medicaid-services-explanationofbenefit-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cms/refs/heads/main/openapi/cms-explanationofbenefit-api-openapi.yml
- filename: cms-patient-api-openapi.yml
  format: yaml
  label: Centers for Medicare and Medicaid Services Patient API
  slug: centers-for-medicare-and-medicaid-services-patient-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cms/refs/heads/main/openapi/cms-patient-api-openapi.yml
certifications: []
description: ''
kind: trust-center
layout: security
name: Cms Trust Center
name_suffix: Trust Center
overview: Centers for Medicare and Medicaid Services maintains a public trust center covering its security and compliance posture.
provider_name: Centers for Medicare and Medicaid Services
provider_slug: cms
slug: cms-trust-center
source_filename: cms-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-15'\nmethod: searched\nsource: https://security.cms.gov/\ntrust_center:\n  published: true\n  name: CMS Information Security and Privacy Program\n  url: https://security.cms.gov/\n  http_status: 200\n  fetched: '2026-08-15'\n  note: >-\n    security.cms.gov is CMS's public information security and privacy program site. It is a federal\n    authorization portal rather than a commercial trust centre — it documents the authorization\n    lifecycle every CMS system (including these APIs) must pass, not a set of purchased attestations.\n    Read it as the CMS equivalent of a trust page, and do not expect SOC 2 or ISO 27001: US federal\n    agencies operate FISMA/FedRAMP authorization instead.\nframeworks:\n  - id: fisma\n    name: Federal Information Security Modernization Act\n    kind: statutory-regime\n    evidence: Listed under Federal Policies & Guidance at https://security.cms.gov/\n  - id: fedramp\n    name: Federal Risk and Authorization Management Program\n\
  \    kind: authorization-program\n    evidence: Listed under Federal Policies & Guidance at https://security.cms.gov/\n  - id: nist-rmf\n    name: NIST Risk Management Framework\n    kind: framework\n    evidence: CMS Risk Management Framework section at https://security.cms.gov/\n  - id: cms-ato\n    name: Authorization to Operate (ATO) / Ongoing Authorization (OA)\n    kind: authorization\n    evidence: System Authorization section at https://security.cms.gov/\n  - id: cms-ars\n    name: CMS Acceptable Risk Safeguards (ARS)\n    kind: control-baseline\n    evidence: CMS Policies & Guidance section at https://security.cms.gov/\n  - id: cms-is2p2\n    name: CMS Information Systems Security and Privacy Policy (IS2P2)\n    kind: policy\n    evidence: CMS Policies & Guidance section at https://security.cms.gov/\n  - id: zero-trust\n    name: Federal Zero Trust strategy\n    kind: strategy\n    evidence: Listed under Federal Policies & Guidance at https://security.cms.gov/\n  - id: hipaa\n\
  \    name: HIPAA Privacy and Security Rules\n    kind: statutory-regime\n    evidence: >-\n      CMS is a HIPAA covered entity and the claims APIs release protected health information under it;\n      the CMS Privacy Program Plan and Privacy Impact Assessment requirements are published at\n      https://security.cms.gov/.\nassurance_artifacts:\n  - name: Privacy Impact Assessment (PIA)\n  - name: System Security and Privacy Plan (SSPP)\n  - name: Information System Risk Assessment (ISRA)\n  - name: Security Impact Analysis (SIA)\n  - name: Plan of Action and Milestones (POA&M)\n  - name: Information System Contingency Plan (ISCP)\n  - name: Cybersecurity and Risk Assessment Program (CSRAP) / penetration testing\n  - name: Continuous Diagnostics and Mitigation (CDM)\ncertifications: []\ncertifications_note: >-\n  No commercial certification (SOC 2, ISO 27001, PCI DSS, HITRUST) is published or claimed, and none\n  should be expected from a federal agency. The equivalent assurance is the\
  \ ATO under FISMA with the\n  NIST-derived CMS ARS control baseline.\nprivacy_policy: https://www.cms.gov/privacy\nvulnerability_disclosure: security/cms-vulnerability-disclosure.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cms/refs/heads/main/security/cms-trust-center.yml
summary_line: trust center published
tags:
- Medicare
- Medicaid
- Healthcare
- Health Insurance
- FHIR
- Federal Government
- Drug Spending
- Provider Data
- Quality Measures
- Claims Data
trust_url: ''
---
