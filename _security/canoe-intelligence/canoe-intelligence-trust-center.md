---
api_specs:
- filename: canoe-intelligence-allocations-api-openapi.yml
  format: yaml
  label: Canoe Intelligence Allocations API
  slug: canoe-intelligence-allocations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/canoe-intelligence/refs/heads/main/openapi/canoe-intelligence-allocations-api-openapi.yml
- filename: canoe-intelligence-authentication-api-openapi.yml
  format: yaml
  label: Canoe Intelligence Authentication API
  slug: canoe-intelligence-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/canoe-intelligence/refs/heads/main/openapi/canoe-intelligence-authentication-api-openapi.yml
- filename: canoe-intelligence-custom-fields-api-openapi.yml
  format: yaml
  label: Canoe Intelligence Custom Fields API
  slug: canoe-intelligence-custom-fields-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/canoe-intelligence/refs/heads/main/openapi/canoe-intelligence-custom-fields-api-openapi.yml
- filename: canoe-intelligence-documents-api-openapi.yml
  format: yaml
  label: Canoe Intelligence Documents API
  slug: canoe-intelligence-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/canoe-intelligence/refs/heads/main/openapi/canoe-intelligence-documents-api-openapi.yml
- filename: canoe-intelligence-funds-api-openapi.yml
  format: yaml
  label: Canoe Intelligence Funds API
  slug: canoe-intelligence-funds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/canoe-intelligence/refs/heads/main/openapi/canoe-intelligence-funds-api-openapi.yml
- filename: canoe-intelligence-organizations-api-openapi.yml
  format: yaml
  label: Canoe Intelligence Organizations API
  slug: canoe-intelligence-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/canoe-intelligence/refs/heads/main/openapi/canoe-intelligence-organizations-api-openapi.yml
- filename: canoe-intelligence-password-grant-tokens-api-openapi.yml
  format: yaml
  label: Canoe Intelligence Password Grant Tokens API
  slug: canoe-intelligence-password-grant-tokens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/canoe-intelligence/refs/heads/main/openapi/canoe-intelligence-password-grant-tokens-api-openapi.yml
- filename: canoe-intelligence-terms-api-openapi.yml
  format: yaml
  label: Canoe Intelligence Terms API
  slug: canoe-intelligence-terms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/canoe-intelligence/refs/heads/main/openapi/canoe-intelligence-terms-api-openapi.yml
- filename: canoe-intelligence-user-api-openapi.yml
  format: yaml
  label: Canoe Intelligence User API
  slug: canoe-intelligence-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/canoe-intelligence/refs/heads/main/openapi/canoe-intelligence-user-api-openapi.yml
certifications:
- SOC 2 Type II
description: ''
kind: trust-center
layout: security
name: Canoe Intelligence Trust Center
name_suffix: Trust Center
overview: Canoe Intelligence maintains a public trust center documenting SOC 2 Type II compliance.
provider_name: Canoe Intelligence
provider_slug: canoe-intelligence
slug: canoe-intelligence-trust-center
source_filename: canoe-intelligence-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-09'\nmethod: searched\nprobe: true\nurl: https://trust.canoeintelligence.com/\nplatform: Vanta\npublic_compliance_page: https://canoeintelligence.com/implementation-data-security/\ncertifications:\n- SOC 2 Type II\ncertification_note: Canoe states on its public Data Security & Implementation page that it \"undergoes an annual\n  SOC2 type 2 audit\". The report itself is behind the Vanta trust-center request flow; no other certification (ISO\n  27001, PCI DSS, HIPAA, FedRAMP) is named on any anonymously reachable Canoe page.\npublished_controls:\n- Principle of least privilege with periodic access review\n- Role-based permissions\n- HTTPS-only platform access\n- Multi-factor authentication enforced\n- Password complexity enforcement\n- API IP filtering\n- Identity federation / SSO (SAML 2.0)\n- User access groups\n- 30-minute session timeout; session id not in the URL\n- Encryption in transit (TLS 1.2+) and at rest (AES-256)\n- Sensitive documents accessible\
  \ only inside the application, never emailed\n- Cloud infrastructure vulnerability scanning\n- Network and web application penetration testing\n- Cloud security configuration assessment\n- Audit logging of all data access and extraction events\n- Data residency controls; on-premise and private-cloud deployment options\n- No model training on client data without explicit contractual authorisation\nevidence:\n- source: https://trust.canoeintelligence.com/\n  status: 200\n  kind: trust-center\n  detail: HTML title \"Canoe Intelligence Trust Center\"; Vanta-hosted SPA (og:image app.vanta.com), content rendered\n    client-side\n- source: https://canoeintelligence.com/implementation-data-security/\n  status: 200\n  kind: compliance-page\n  keywords:\n  - SOC2 type 2\n  - penetration testing\n  - MFA\n  - least privilege\n  - encryption\n- source: https://canoeintelligence.com/llms-full.txt\n  status: 200\n  kind: llms-full\n  detail: '\"Key management aligned with SOC 2 Type II requirements\"\
  '\nnote: probe-security-programs.py recorded trust=none because the Vanta trust center renders client-side and its\n  served HTML carries no compliance keywords. The trust center is real and was verified by hand; the certification\n  list is limited to what Canoe states on anonymously readable pages.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/canoe-intelligence/refs/heads/main/security/canoe-intelligence-trust-center.yml
summary_line: SOC 2 Type II
tags:
- Alternative Investments
- Private Markets
- Document Automation
- Data Extraction
- Fund Administration
- capital-calls
- k-1-tax-documents
- Portfolio Reporting
- Financial-Services
- Fintech
- Wealth Management
- Institutional Investors
trust_url: https://trust.canoeintelligence.com/
---
