---
api_specs:
- filename: docontrol-authentication-api-openapi.yml
  format: yaml
  label: DoControl Authentication API
  slug: docontrol-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/docontrol/refs/heads/main/openapi/docontrol-authentication-api-openapi.yml
- filename: docontrol-graphql-api-openapi.yml
  format: yaml
  label: DoControl GraphQL API
  slug: docontrol-graphql-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/docontrol/refs/heads/main/openapi/docontrol-graphql-api-openapi.yml
certification_count: 4
certifications:
- ISO 27001
- SOC 2 Type II
- HIPAA
- GDPR
description: Certifications read from DoControl's own documentation page, which names them in plain text. This file was briefly overwritten on 2026-09-06 by an automated keyword probe that could only see HIPAA and GDPR — the marketing /security page is a JS-rendered Webflow page whose certification copy is not in the served HTML, so the probe found less than DoControl actually publishes. The documentation page is the stronger source and is used here.
kind: trust-center
layout: security
name: Docontrol Trust Center
name_suffix: Trust Center
overview: DoControl maintains a public trust center documenting ISO 27001, SOC 2 Type II, HIPAA, and GDPR compliance.
provider_name: DoControl
provider_slug: docontrol
slug: docontrol-trust-center
source_filename: docontrol-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-09-06'\nmethod: searched\nprobe: true\nsource: https://docs.docontrol.io/docontrol-user-guide/getting-started/overview/security-privacy-and-compliance.md\nurl: https://www.docontrol.io/security\ndescription: >-\n  Certifications read from DoControl's own documentation page, which names them in plain text.\n  This file was briefly overwritten on 2026-09-06 by an automated keyword probe that could only\n  see HIPAA and GDPR — the marketing /security page is a JS-rendered Webflow page whose\n  certification copy is not in the served HTML, so the probe found less than DoControl actually\n  publishes. The documentation page is the stronger source and is used here.\ncertifications:\n- id: iso-27001\n  name: ISO 27001\n  evidence: 'Documentation states: \"Compliance certifications (ISO 27001, SOC2 type II)\"'\n  source: https://docs.docontrol.io/docontrol-user-guide/getting-started/overview/security-privacy-and-compliance.md\n- id: soc2-type-ii\n  name: SOC 2 Type\
  \ II\n  evidence: 'Documentation states: \"Compliance certifications (ISO 27001, SOC2 type II)\"'\n  source: https://docs.docontrol.io/docontrol-user-guide/getting-started/overview/security-privacy-and-compliance.md\n- id: hipaa\n  name: HIPAA\n  evidence: HIPAA compliance claimed on the DoControl website.\n  source: https://www.docontrol.io/\n- id: gdpr\n  name: GDPR\n  evidence: GDPR readiness claimed on the DoControl website.\n  source: https://www.docontrol.io/\nprogramme:\n  page: https://www.docontrol.io/security\n  page_status: 200\n  page_machine_readable: false\n  page_note: >-\n    Webflow, client-rendered. HTTP 200 and 120KB of HTML, but the certification names are not in\n    the served markup — a crawler reading only the response body sees none of them.\n  contact: security@docontrol.io\n  practices:\n  - Penetration testing\n  - Publicly available self-assessments\n  - Data processing addendum\n  - Information Security Policy\n  data_handling:\n    llm_use_disclosed: true\n\
  \    llm_statement: >-\n      DoControl discloses that it uses LLMs for global search, alerts and its Dot assistant, that\n      the models are hosted inside DoControl's own environment with no internet access, and that\n      customer data is never sent to, stored by, or used to train any external LLM or AI service.\n    source: https://docs.docontrol.io/docontrol-user-guide/getting-started/overview/security-privacy-and-compliance.md\ntrust_center:\n  dedicated_portal: false\n  note: >-\n    No Vanta/Drata/SafeBase-style trust portal; trust.docontrol.io does not resolve. Evidence is a\n    marketing page plus a documentation page, with no downloadable report index.\nevidence:\n- source: https://docs.docontrol.io/docontrol-user-guide/getting-started/overview/security-privacy-and-compliance.md\n  status: 200\n  keywords:\n  - iso 27001\n  - soc2 type ii\n  - penetration testing\n  - self-assessments\n  - data processing addendum\n- source: https://www.docontrol.io/\n  status: 200\n  keywords:\n\
  \  - hipaa\n  - gdpr\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/docontrol/refs/heads/main/security/docontrol-trust-center.yml
summary_line: ISO 27001, SOC 2 Type II, HIPAA, GDPR
tags:
- Data Security
- SaaS Security
- Data Access Governance
- Data Loss Prevention
- Insider Risk Management
- SSPM
- GraphQL
- MCP
trust_url: https://www.docontrol.io/security
---
