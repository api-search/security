---
api_specs:
- filename: cb-insights-authorization-api-openapi.yml
  format: yaml
  label: CB Insights Authorization API
  slug: cb-insights-authorization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cb-insights/refs/heads/main/openapi/cb-insights-authorization-api-openapi.yml
- filename: cb-insights-businessrelationships-api-openapi.yml
  format: yaml
  label: CB Insights Business Relationships API
  slug: cb-insights-businessrelationships-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cb-insights/refs/heads/main/openapi/cb-insights-businessrelationships-api-openapi.yml
- filename: cb-insights-chatcbi-api-openapi.yml
  format: yaml
  label: CB Insights Chat CBI API
  slug: cb-insights-chatcbi-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cb-insights/refs/heads/main/openapi/cb-insights-chatcbi-api-openapi.yml
- filename: cb-insights-financialtransactions-api-openapi.yml
  format: yaml
  label: CB Insights Financial Transactions API
  slug: cb-insights-financialtransactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cb-insights/refs/heads/main/openapi/cb-insights-financialtransactions-api-openapi.yml
- filename: cb-insights-firmographics-api-openapi.yml
  format: yaml
  label: CB Insights Firmographics API
  slug: cb-insights-firmographics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cb-insights/refs/heads/main/openapi/cb-insights-firmographics-api-openapi.yml
- filename: cb-insights-managementandboard-api-openapi.yml
  format: yaml
  label: CB Insights Management And Board API
  slug: cb-insights-managementandboard-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cb-insights/refs/heads/main/openapi/cb-insights-managementandboard-api-openapi.yml
- filename: cb-insights-organizations-api-openapi.yml
  format: yaml
  label: CB Insights Organizations API
  slug: cb-insights-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cb-insights/refs/heads/main/openapi/cb-insights-organizations-api-openapi.yml
- filename: cb-insights-outlook-api-openapi.yml
  format: yaml
  label: CB Insights Outlook API
  slug: cb-insights-outlook-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cb-insights/refs/heads/main/openapi/cb-insights-outlook-api-openapi.yml
- filename: cb-insights-revenue-api-openapi.yml
  format: yaml
  label: CB Insights Revenue API
  slug: cb-insights-revenue-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cb-insights/refs/heads/main/openapi/cb-insights-revenue-api-openapi.yml
- filename: cb-insights-scoutingreports-api-openapi.yml
  format: yaml
  label: CB Insights Scouting Reports API
  slug: cb-insights-scoutingreports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cb-insights/refs/heads/main/openapi/cb-insights-scoutingreports-api-openapi.yml
- filename: cb-insights-strategymap-api-openapi.yml
  format: yaml
  label: CB Insights Strategy Map API
  slug: cb-insights-strategymap-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cb-insights/refs/heads/main/openapi/cb-insights-strategymap-api-openapi.yml
certifications:
- SOC 2 Type II
- GDPR
- CCPA
- EU AI Act (deployer obligations)
description: ''
kind: trust-center
layout: security
name: Cb Insights Trust Center
name_suffix: Trust Center
overview: CB Insights maintains a public trust center documenting SOC 2 Type II, GDPR, CCPA, and EU AI Act (deployer obligations) compliance.
provider_name: CB Insights
provider_slug: cb-insights
slug: cb-insights-trust-center
source_filename: cb-insights-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-09'\nmethod: searched\nsource: https://trust.cbinsights.com/\ndocs:\n- https://trust.cbinsights.com/\n- https://www.cbinsights.com/security-and-privacy/\n- https://www.cbinsights.com/security/\ntrust_center:\n  url: https://trust.cbinsights.com/\n  platform: Vanta\n  http_status: 200\n  page_title: CB Insights Trust Center\n  machine_readable: false\n  readability_note: >-\n    The trust center is a Vanta-hosted single-page app. It serves the same HTML shell with HTTP 200\n    for EVERY path on the host — /api/*, /trpc/*, invented paths — so a 200 there is not evidence\n    that any particular document exists, and the certification list, control set and document\n    requests all render client-side and could not be read without a browser. Certifications below\n    are therefore taken from CB Insights' own server-rendered security page, not from the trust\n    center.\n  access: >-\n    Reports appear to be gated behind a document request (an app.vanta.com/doc?s=...\
  \ link is present\n    in the page shell); no report is downloadable anonymously.\ncertifications:\n- name: SOC 2 Type II\n  status: certified\n  evidence: '\"Our infrastructure is audited and certified to meet the most rigorous standards for data security.\"'\n  source: https://www.cbinsights.com/security-and-privacy/\n- name: GDPR\n  status: compliant\n  evidence: '\"We meet the strict requirements of the General Data Protection Regulation for data privacy and protection.\"'\n  source: https://www.cbinsights.com/security-and-privacy/\n- name: CCPA\n  status: in-progress\n  evidence: '\"We''re actively preparing to meet CCPA standards.\"'\n  source: https://www.cbinsights.com/security-and-privacy/\n- name: EU AI Act (deployer obligations)\n  status: in-progress\n  evidence: '\"...and the EU AI Act for deployers.\"'\n  source: https://www.cbinsights.com/security-and-privacy/\nnot_claimed:\n- ISO 27001\n- HIPAA\n- PCI DSS\n- FedRAMP\nsecurity_controls_published:\n- AES 256-bit encryption\
  \ at rest\n- TLS 1.2 in transit\n- full audit trail of activity\n- granular administrative controls on AI features\n- SSO, MFA and role-based access control\n- AI hallucination testing and observability\nai_data_use:\n  statement: '\"Your data is never used to train the AI models we use. Period.\"'\n  source: https://www.cbinsights.com/security-and-privacy/\nvulnerability_disclosure:\n  published: false\n  probed:\n  - url: https://www.cbinsights.com/.well-known/security.txt\n    status: 404\n  - url: https://api-docs.cbinsights.com/.well-known/security.txt\n    status: 404\n  - url: https://mcp.cbinsights.com/.well-known/security.txt\n    status: 404\n  - url: https://api.cbinsights.com/.well-known/security.txt\n    status: 401\n  note: >-\n    No security.txt, no responsible-disclosure page, and no bug-bounty program (HackerOne, Bugcrowd\n    or Intigriti) was found. The published security page names no security contact address; the only\n    documented contact anywhere in the estate\
  \ is the general info@cbinsights.com.\ncross_links:\n  conformance: conformance/cb-insights-conformance.yml\n  domain_security: security/cb-insights-domain-security.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cb-insights/refs/heads/main/security/cb-insights-trust-center.yml
summary_line: SOC 2 Type II, GDPR, CCPA, EU AI Act (deployer obligations)
tags:
- Company
- Market Intelligence
- private-company-data
- Venture Capital
- funding-data
- investor-data
- Company Data
- People Data
- BusinessRelationships
- predictive-scoring
- MCP
- agent-native
- Data Enrichment
- Snowflake
trust_url: ''
---
