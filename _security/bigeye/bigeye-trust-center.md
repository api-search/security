---
api_specs:
- filename: bigeye-metadata-openapi.json
  format: json
  label: Bigeye Metadata API
  slug: bigeye-metadata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bigeye/refs/heads/main/openapi/bigeye-metadata-openapi.json
- filename: bigeye-observability-openapi.json
  format: json
  label: Bigeye Observability API
  slug: bigeye-observability-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bigeye/refs/heads/main/openapi/bigeye-observability-openapi.json
- filename: bigeye-sensitivity-openapi.json
  format: json
  label: Bigeye Sensitivity API
  slug: bigeye-sensitivity-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bigeye/refs/heads/main/openapi/bigeye-sensitivity-openapi.json
certifications:
- SOC 2 Type 2
- ISO 27001
description: ''
kind: trust-center
layout: security
name: Bigeye Trust Center
name_suffix: Trust Center
overview: Bigeye maintains a public trust center documenting SOC 2 Type 2 and ISO 27001 compliance.
provider_name: Bigeye
provider_slug: bigeye
slug: bigeye-trust-center
source_filename: bigeye-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-02'\nmethod: searched\nprobe: true\nsource: https://www.bigeye.com/platform/security\nurl: https://www.bigeye.com/platform/security\nalternate_urls:\n- url: https://trust.bigeye.com/\n  status: 200\n  note: >-\n    A trust.bigeye.com host resolves and returns 200, but the page is a\n    client-rendered shell that exposes no certification names, no document\n    request flow and no disclosure policy to an anonymous fetch. The\n    substantive, machine-readable compliance content lives on the two URLs\n    recorded above.\n- url: https://docs.bigeye.com/docs/security-and-compliance\n  status: 200\n  role: primary detail page\ncertifications:\n- id: soc2-type-2\n  name: SOC 2 Type 2\n  evidence: '\"SOC 2 Type 2 Report\" listed under Security Certification; \"Bigeye is\n    a fully managed SOC 2 and ISO 27001 compliant SaaS application.\"'\n- id: iso-27001\n  name: ISO 27001\n  evidence: '\"ISO 27001 Certification\" listed under Security Certification.'\nreports_available_on_request:\n\
  - SOC 2 Type 2 report\n- Penetration test report\n- Data Processing Addendum (DPA)\ncontrols:\n  hosting: AWS\n  encryption_at_rest: AES-256 (AWS-managed RDS)\n  encryption_in_transit: TLS v1.2 or higher\n  sso_provider: Auth0\n  enterprise_sso: [Okta, Ping Identity, Azure AD]\n  private_networking: AWS PrivateLink (Bigeye Enterprise)\n  waf: AWS WAF Security Automation\n  background_checks: Checkr\n  penetration_testing: annual, third party, application layer\n  data_minimization: >-\n    Bigeye extracts only aggregate statistics, query logs and metadata; raw data\n    never leaves the customer's production environment. Warehouse connections\n    use read-only service accounts over JDBC.\n  credential_handling: >-\n    Direct-connection credentials are encrypted at rest on Bigeye's AWS\n    infrastructure and are not accessible to Bigeye engineers. Agent-connection\n    credentials never leave the customer's infrastructure.\nsecurity_contact: security@bigeye.com\nevidence:\n- source:\
  \ https://www.bigeye.com/platform/security\n  fetched: '2026-08-02'\n  http_status: 200\n  keywords: [soc 2, soc2, iso 27001, penetration, encryption, security@]\n- source: https://docs.bigeye.com/docs/security-and-compliance\n  fetched: '2026-08-02'\n  http_status: 200\n  keywords: [soc 2 type 2 report, iso 27001 certification, aws, checkr, auth0, aes-256,\n    aws waf]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bigeye/refs/heads/main/security/bigeye-trust-center.yml
summary_line: SOC 2 Type 2, ISO 27001
tags:
- Company
- Data Observability
- Data Quality
- Data Lineage
- Data Governance
- Metadata Management
- Data Catalog
- Sensitive Data Discovery
- Monitoring
- Analytics
- AI Trust
- Snowflake
- Databricks
trust_url: https://www.bigeye.com/platform/security
---
