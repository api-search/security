---
api_specs:
- filename: leadspace-authorization-api-openapi.yml
  format: yaml
  label: Leadspace Authorization API
  slug: leadspace-authorization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leadspace/refs/heads/main/openapi/leadspace-authorization-api-openapi.yml
- filename: leadspace-discovery-api-openapi.yml
  format: yaml
  label: Leadspace Discovery API
  slug: leadspace-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leadspace/refs/heads/main/openapi/leadspace-discovery-api-openapi.yml
- filename: leadspace-enrichment-api-openapi.yml
  format: yaml
  label: Leadspace Enrichment API
  slug: leadspace-enrichment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leadspace/refs/heads/main/openapi/leadspace-enrichment-api-openapi.yml
- filename: leadspace-intent-api-openapi.yml
  format: yaml
  label: Leadspace Intent API
  slug: leadspace-intent-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leadspace/refs/heads/main/openapi/leadspace-intent-api-openapi.yml
- filename: leadspace-results-api-openapi.yml
  format: yaml
  label: Leadspace Results API
  slug: leadspace-results-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leadspace/refs/heads/main/openapi/leadspace-results-api-openapi.yml
certifications:
- SOC 2 Type II
- ISO 27001
description: Leadspace runs no dedicated trust portal (trust.leadspace.com and security.leadspace.com do not resolve; /trust, /security and /compliance 404). It does publish a first-party Security and Compliance page on the product site naming specific certifications and regulatory regimes, plus a long-standing General Statement of Information Security and Privacy in the help center. Those two pages are the trust surface, and they are recorded here rather than claimed as a trust center that does not exist.
kind: trust-center
layout: security
name: Leadspace Trust Center
name_suffix: Trust Center
overview: Leadspace maintains a public trust center documenting SOC 2 Type II and ISO 27001 compliance.
provider_name: Leadspace
provider_slug: leadspace
slug: leadspace-trust-center
source_filename: leadspace-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nprobe: true\nurl: https://www.leadspace.com/platform/security-and-compliance\ndescription: >-\n  Leadspace runs no dedicated trust portal (trust.leadspace.com and\n  security.leadspace.com do not resolve; /trust, /security and /compliance 404).\n  It does publish a first-party Security and Compliance page on the product site\n  naming specific certifications and regulatory regimes, plus a long-standing\n  General Statement of Information Security and Privacy in the help center.\n  Those two pages are the trust surface, and they are recorded here rather than\n  claimed as a trust center that does not exist.\ntrust_portal:\n  present: false\n  probed:\n  - url: https://trust.leadspace.com/\n    status: 000\n    note: DNS does not resolve\n  - url: https://security.leadspace.com/\n    status: 000\n    note: DNS does not resolve\n  - url: https://www.leadspace.com/trust\n    status: 404\n  - url: https://www.leadspace.com/security\n  \
  \  status: 404\n  - url: https://www.leadspace.com/compliance\n    status: 404\ncertifications:\n- SOC 2 Type II\n- ISO 27001\nregulations:\n- GDPR\n- CCPA\n- Texas Data Broker registration\ncontrols_published:\n- Secure cloud architecture\n- Encrypted data storage and transfer\n- Continuous vulnerability monitoring\n- Role-based access control\n- Multi-layer authentication\n- Robust incident management\n- Data minimization best practices\n- Purpose-driven data use\n- Consent-aware processing\n- Strict retention and deletion standards\n- Automated system checks and security alerts\n- Real-time anomaly detection\n- Continuous compliance audits\n- Regular penetration testing\nprivacy_rights:\n  do_not_sell: https://www.leadspace.com/do-not-sell-form\n  texas_data_broker_notice: https://www.leadspace.com/texas-data-broker-notice\n  privacy_notice: https://www.leadspace.com/privacy-notice\n  cookie_notice: https://www.leadspace.com/cookie-notice\n  data_processing_addendum: https://www.leadspace.com/leadspace-data-processing-addendum/\n\
  \  note: >-\n    Material for a B2B data provider: Leadspace sells identity data about\n    individuals, so the Do Not Sell form and the Texas data-broker notice are\n    part of its compliance posture, not boilerplate.\nvulnerability_disclosure: security/leadspace-vulnerability-disclosure.yml\nevidence:\n- source: https://www.leadspace.com/platform/security-and-compliance\n  status: 200\n  keywords:\n  - SOC 2 Type II\n  - GDPR\n  - CCPA\n  - penetration testing\n  - role-based access control\n  - encrypted data storage and transfer\n  fetched: '2026-08-13'\n- source: https://support.leadspace.com/hc/en-us/articles/360012276859-General-Statement-of-Information-Security-and-Privacy\n  kind: help-center-security-statement\n  note: >-\n    Cited from the 2026-07-19 pass (ISO 27001 certified, SOC 2 Type II audited).\n    Re-probe on 2026-08-13 returned 403 — the Zendesk help center now blocks\n    automated fetches, so this URL is retained as previously verified rather\n    than re-verified.\n\
  gaps:\n- No trust portal with downloadable, current audit reports or a subprocessor list; certifications are asserted in marketing prose rather than evidenced by a report request flow.\n- The Security and Compliance page names SOC 2 Type II but does not state the audit period or the auditor.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/leadspace/refs/heads/main/security/leadspace-trust-center.yml
summary_line: SOC 2 Type II, ISO 27001
tags:
- MCP
- AI Agents
- B2B Data
- Customer Data Platform
- Data Enrichment
- Intent Data
- Sales Intelligence
- Account-Based Marketing
- Identity Resolution
- Firmographics
- Lead Scoring
- Company
trust_url: https://www.leadspace.com/platform/security-and-compliance
---
