---
api_specs:
- filename: redocly-search-api-openapi.yaml
  format: yaml
  label: Redocly Realm Search API
  slug: redocly-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/redocly/refs/heads/main/openapi/redocly-search-api-openapi.yaml
- filename: redocly-docs-mcp-openapi.yaml
  format: yaml
  label: Redocly Docs MCP Server
  slug: redocly-docs-mcp
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/redocly/refs/heads/main/openapi/redocly-docs-mcp-openapi.yaml
- filename: redocly-scout-openapi.yaml
  format: yaml
  label: Redocly Scout API
  slug: redocly-scout
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/redocly/refs/heads/main/openapi/redocly-scout-openapi.yaml
- filename: redocly-scout-agent-openapi.yaml
  format: yaml
  label: Redocly Scout Agent API
  slug: redocly-scout-agent
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/redocly/refs/heads/main/openapi/redocly-scout-agent-openapi.yaml
certifications:
- SOC 2 Type II
- CSA STAR / CAIQ v4
- PCI DSS
- GDPR / CCPA
description: Redocly publishes a single security page rather than a hosted trust portal, and it names concrete certifications with concrete dates. The compliance ARTIFACTS themselves — SOC 2 Type II report, penetration test results — are gated behind a Reunite login on the Compliance page, so the claims are public and the evidence is customer-only.
kind: trust-center
layout: security
name: Redocly Trust Center
name_suffix: Trust Center
overview: Redocly maintains a public trust center documenting SOC 2 Type II, CSA STAR / CAIQ v4, PCI DSS, and GDPR / CCPA compliance.
provider_name: Redocly
provider_slug: redocly
slug: redocly-trust-center
source_filename: redocly-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-27'\nmethod: searched\nsource: >-\n  https://redocly.com/security (fetched 2026-08-27, HTTP 200),\n  https://redocly.com/sub-processors, https://redocly.com/dpa and\n  https://redocly.com/docs/realm/reunite/organization/access-compliance-reports.\nprovider: Redocly\nproviderId: redocly\nname: Security at Redocly\nurl: https://redocly.com/security\ndescription: >-\n  Redocly publishes a single security page rather than a hosted trust portal,\n  and it names concrete certifications with concrete dates. The compliance\n  ARTIFACTS themselves — SOC 2 Type II report, penetration test results — are\n  gated behind a Reunite login on the Compliance page, so the claims are\n  public and the evidence is customer-only.\ncertifications:\n  - name: SOC 2 Type II\n    status: completed\n    evidence: >-\n      \"Redocly has completed the System and Organization Controls (SOC) 2,\n      Type II audit. Log in to download this and other reports.\"\n    report_access: https://redocly.com/docs/realm/reunite/organization/access-compliance-reports\n\
  \    gated: true\n  - name: CSA STAR / CAIQ v4\n    status: certified\n    evidence: >-\n      \"Completed the CAIQ version 4 questionnaire and certified under the\n      Cloud Security Alliance's (CSA) STAR program for cybersecurity.\"\n  - name: PCI DSS\n    status: inherited\n    evidence: >-\n      Redocly does not store or process payment information; it relies on\n      Stripe and Rebilly, both PCI DSS Level 1 service providers.\n  - name: GDPR / CCPA\n    status: addressed-by-dpa\n    evidence: Data Processing Addendum published at https://redocly.com/dpa\npractices:\n  encryption:\n    in_transit: TLS 1.2+\n    at_rest: AES-256\n  identity:\n    sso: [SAML 2.0, OpenID Connect]\n    domain_verification: true\n    rbac: Project-level permissions for groups; IdP-attribute team mapping.\n    audit_trail: Event logging of project updates over time.\n  testing:\n    penetration_testing: Internal and third-party, at least annually.\n    vulnerability_management: >-\n      Daily code and\
  \ dependency scanning via AWS Elastic Container Registry;\n      critical issues resolved in under one week.\n    malware_protection: Continuous container monitoring via AWS ECR plus device agents.\n  people:\n    background_checks: true\n    security_awareness_training: true\n    least_privilege: true\n  availability:\n    waf: true\n    rpo_minutes: 10\n    rto_minutes: 30\n    dr_last_tested: '2026-06-25'\n    status_page: https://status.redocly.com/\n    sla: https://redocly.com/sla\n  infrastructure:\n    hosting: AWS\n    sub_processors: https://redocly.com/sub-processors\n    named_sub_processors:\n      - name: AWS\n        location: US\n        role: All services, email service provider, storage and processing\n      - name: Google\n        location: US\n        role: LLM provider for AI search and AI assistant features\n      - name: ClickHouse, Inc.\n        location: US\n        role: Analytics data\n      - name: Auth0\n        location: US\n        role: Identity provider\
  \ for login and registration (Redocly Workflows only)\ndata_ownership:\n  statement: >-\n    Redocly states that every code sample, page and asset a customer creates\n    belongs to the customer.\n  privacy_notice: https://redocly.com/privacy-notice\ngaps:\n  - No hosted trust center (Vanta/Drata/SafeBase style) with self-serve document access.\n  - Compliance reports require a Reunite login; there is no NDA-gated public request flow described.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/redocly/refs/heads/main/security/redocly-trust-center.yml
summary_line: SOC 2 Type II, CSA STAR / CAIQ v4, PCI DSS, GDPR / CCPA
tags:
- Artificial Intelligence
- API Catalog
- API Documentation
- Arazzo
- Developer Portal
- Governance
- Linting
- MCP
- Monitoring
- OpenAPI
trust_url: https://redocly.com/security
---
