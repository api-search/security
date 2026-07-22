---
api_specs:
- filename: unblocked-public-api-openapi-original.json
  format: json
  label: Unblocked Public API
  slug: unblocked-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unblocked/refs/heads/main/openapi/unblocked-public-api-openapi-original.json
certifications:
- SOC 2 Type II
- SOC 3
- CASA Tier 2
- GDPR
description: Unblocked (legal entity Next Chapter Software Inc) operates a SafeBase trust center at trust.getunblocked.com, linked from the security page at getunblocked.com/security. It lists compliance certifications and gated documents (pentest report, cyber insurance, policies for backup, BC/DR, data classification/protection/retention, encryption, subprocessors, DPA) plus AI-specific sections (AI Security, AI Monitoring, AI Risk Management).
kind: trust-center
layout: security
name: Unblocked Trust Center
name_suffix: Trust Center
overview: Unblocked maintains a public trust center documenting SOC 2 Type II, SOC 3, CASA Tier 2, and GDPR compliance.
provider_name: Unblocked
provider_slug: unblocked
slug: unblocked-trust-center
source_filename: unblocked-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nprobe: true\nsource: https://trust.getunblocked.com/\nurl: https://trust.getunblocked.com/\ndescription: >-\n  Unblocked (legal entity Next Chapter Software Inc) operates a SafeBase trust\n  center at trust.getunblocked.com, linked from the security page at\n  getunblocked.com/security. It lists compliance certifications and gated\n  documents (pentest report, cyber insurance, policies for backup, BC/DR,\n  data classification/protection/retention, encryption, subprocessors, DPA)\n  plus AI-specific sections (AI Security, AI Monitoring, AI Risk Management).\nlegal_entity: Next Chapter Software Inc\nplatform: SafeBase\ncertifications:\n- SOC 2 Type II\n- SOC 3\n- CASA Tier 2\n- GDPR\nsecurity_page:\n  url: https://getunblocked.com/security/\n  highlights:\n    - TLS in transit; encryption at rest with AWS-managed keys; customer-specific keys across network layers.\n    - Customer data never used to train shared models; data removed\
  \ on deletion.\n    - No stored passwords; authentication via SAML SSO or OAuth 2.0 to the customer identity provider.\n    - Ongoing penetration testing, static/dynamic scans, code scanning; background checks and security training for employees.\nevidence:\n- source: https://trust.getunblocked.com/\n  keywords:\n  - soc 2 type 2\n  - soc 3\n  - casa tier 2\n  - gdpr\n  - trust center\n  - penetration testing\n- source: https://getunblocked.com/security/\n  keywords:\n  - SOC 2 Type II\n  - CASA Tier II\n  - GDPR\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/unblocked/refs/heads/main/security/unblocked-trust-center.yml
summary_line: SOC 2 Type II, SOC 3, CASA Tier 2, GDPR
tags:
- Company
- Developer Tools
- AI
- Developer Experience
- Knowledge Management
- Code Review
- MCP
- AI Agents
- Context Engineering
- Search
trust_url: https://trust.getunblocked.com/
---
