---
api_specs:
- filename: edgee-chat-api-openapi.yml
  format: yaml
  label: Edgee Chat API
  slug: edgee-chat-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/edgee/refs/heads/main/openapi/edgee-chat-api-openapi.yml
- filename: edgee-compress-api-openapi.yml
  format: yaml
  label: Edgee Compress API
  slug: edgee-compress-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/edgee/refs/heads/main/openapi/edgee-compress-api-openapi.yml
- filename: edgee-messages-api-openapi.yml
  format: yaml
  label: Edgee Messages API
  slug: edgee-messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/edgee/refs/heads/main/openapi/edgee-messages-api-openapi.yml
- filename: edgee-models-api-openapi.yml
  format: yaml
  label: Edgee Models API
  slug: edgee-models-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/edgee/refs/heads/main/openapi/edgee-models-api-openapi.yml
- filename: edgee-responses-api-openapi.yml
  format: yaml
  label: Edgee Responses API
  slug: edgee-responses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/edgee/refs/heads/main/openapi/edgee-responses-api-openapi.yml
- filename: edgee-tokens-api-openapi.yml
  format: yaml
  label: Edgee Tokens API
  slug: edgee-tokens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/edgee/refs/heads/main/openapi/edgee-tokens-api-openapi.yml
certifications:
- SOC 2 Type 1
- SOC 2 Type 2
description: ''
kind: trust-center
layout: security
name: Edgee Trust Center
name_suffix: Trust Center
overview: Edgee maintains a public trust center documenting SOC 2 Type 1 and SOC 2 Type 2 compliance.
provider_name: Edgee
provider_slug: edgee
slug: edgee-trust-center
source_filename: edgee-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-17'\nmethod: searched\nprobe: false\nurl: https://trust.edgee.ai/\nhttp_status: 200\nfetched: '2026-08-17'\nentity: Edgee Corporation\nplatform: Bastion\ncertifications:\n- SOC 2 Type 1\n- SOC 2 Type 2\ncontrols:\n  total: 82\n  categories: [Business Operations, Cloud Security, Human Resources, Data Protection]\n  note: Control counts read from the live trust center on 2026-08-17; they move as the program is\n    refreshed.\nsubprocessors:\n  count: 5\n  listed: true\n  names_captured: false\n  note: The trust center states a subprocessor list of 5 exists; the names are behind the \"View all\"\n    control and were not captured.\nrelated_pages:\n- {name: Data Processing Agreement, url: 'https://www.edgee.ai/dpa', http_status: 200}\n- {name: Privacy Policy, url: 'https://www.edgee.ai/privacy', http_status: 200}\n- {name: Terms, url: 'https://www.edgee.ai/terms', http_status: 200}\nenterprise_controls:\n  source: https://www.edgee.ai/pricing\n  offered: [SSO/SAML\
  \ authentication, Private gateway (SaaS or on-premises), Custom data residency\n      (EU or US), 'Custom privacy controls including PII redaction']\n  note: Offered as Enterprise-tier features rather than as a published security posture.\nvulnerability_disclosure:\n  found: false\n  note: 'No security.txt (404 on every host), no /security, /trust or /responsible-disclosure page\n    (404), no bug bounty program on HackerOne / Bugcrowd / Intigriti found, and no security@ contact\n    published. probe-security-programs.py returned vdp=none. Recorded as an absence — no Security or\n    VulnerabilityDisclosure pointer is wired in apis.yml. This is the clearest single gap in Edgee''s\n    otherwise credible security posture: a company with a SOC 2 Type 2 and no published way to report\n    a vulnerability.'\n  evidence:\n  - {url: 'https://www.edgee.ai/.well-known/security.txt', http_status: 404}\n  - {url: 'https://edgee.io/.well-known/security.txt', http_status: 404}\n  - {url: 'https://api.edgee.app/.well-known/security.txt',\
  \ http_status: 404}\n  - {url: 'https://www.edgee.ai/security', http_status: 404}\n  - {url: 'https://www.edgee.ai/trust', http_status: 404}\nevidence:\n- {source: 'https://trust.edgee.ai/', keywords: [SOC 2 Type 2, SOC 2 Type 1, trust center,\n      subprocessors, controls], fetched: '2026-08-17'}\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/edgee/refs/heads/main/security/edgee-trust-center.yml
summary_line: SOC 2 Type 1, SOC 2 Type 2
tags:
- Company
- Artificial Intelligence
- LLM
- AI Gateway
- Agents
- Developer Tools
- Observability
- FinOps
- Edge Computing
- Cost Management
trust_url: https://trust.edgee.ai/
---
