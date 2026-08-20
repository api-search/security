---
api_specs:
- filename: happyrobot-public-api-openapi.json
  format: json
  label: Happyrobot Public API
  slug: happyrobot-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/happyrobot/refs/heads/main/openapi/happyrobot-public-api-openapi.json
- filename: happyrobot-platform-v1-openapi.json
  format: json
  label: Happyrobot Platform API v1
  slug: happyrobot-platform-api-v1
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/happyrobot/refs/heads/main/openapi/happyrobot-platform-v1-openapi.json
- filename: happyrobot-public-api-openapi.json
  format: json
  label: Happyrobot Public API (EU cluster)
  slug: happyrobot-public-api-eu-cluster
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/happyrobot/refs/heads/main/openapi/happyrobot-public-api-openapi.json
certifications:
- SOC 2 Type II
- GDPR
- HIPAA
- EU AI Act
- NIST CSF
- DORA
description: ''
kind: trust-center
layout: security
name: Happyrobot Trust Center
name_suffix: Trust Center
overview: Happyrobot maintains a public trust center documenting SOC 2 Type II, GDPR, HIPAA, EU AI Act, NIST CSF, and DORA compliance.
provider_name: Happyrobot
provider_slug: happyrobot
slug: happyrobot-trust-center
source_filename: happyrobot-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-01'\nmethod: searched\nprobe: true\nurl: https://trust.happyrobot.ai/\nplatform: Vanta\nnotes: >-\n  trust.happyrobot.ai returns HTTP 200 and is served from Vanta's hosted trust-report application\n  (content-location: assets.vanta.com/static/index-trust-report.<hash>.html). The report body is rendered\n  client-side, so the certification list could not be read from the HTML directly. The frameworks below\n  are therefore taken from Happyrobot's own public security page, which is server-rendered and readable,\n  and the trust center is recorded as present and Vanta-operated.\ncertifications:\n- SOC 2 Type II\n- GDPR\n- HIPAA\n- EU AI Act\n- NIST CSF\n- DORA\ncertifications_source: https://www.happyrobot.ai/product/security-and-reliability\nattestation_access: >-\n  Compliance documentation is stated to be \"available to qualified customers under NDA\" — reports are not\n  downloadable from the public trust center without a request.\nsecurity_posture_claims:\n\
  - end-to-end encryption with per-workflow retention policies\n- zero-trust network architecture\n- role-based access control (Owner, Editor, Viewer)\n- per-customer encryption keys on dedicated deployments\n- automatic model failover across LLM, TTS and STT providers\n- multi-availability-zone infrastructure with automatic failover\n- in-country data residency\n- customer data never used to train models and never shared across tenants\nindependently_verified:\n- claim: in-country data residency\n  verification: >-\n    A complete EU cluster exists and answers independently — platform.eu.happyrobot.ai serves its own\n    OpenAPI (200) and its own RFC 8414 authorization server, and mcp.platform.eu.happyrobot.ai serves its\n    own MCP endpoints.\n- claim: role-based access control\n  verification: >-\n    Reflected in the Public API — org membership operations plus 403 responses declared on 20 operations.\n- claim: TLS everywhere\n  verification: >-\n    TLSv1.3 with HSTS max-age 63072000\
  \ on www.happyrobot.ai and docs.happyrobot.ai; see\n    security/happyrobot-domain-security.yml.\nevidence:\n- source: https://trust.happyrobot.ai/\n  http_status: 200\n  keywords:\n  - vanta\n  - trust center\n  note: 13 references to Vanta in the delivered document; body is client-rendered\n- source: https://www.happyrobot.ai/product/security-and-reliability\n  http_status: 200\n  keywords:\n  - SOC 2 Type II\n  - GDPR\n  - HIPAA\n  - EU AI Act\n  - NIST CSF\n  - DORA\nx-evidence:\n  fetched: '2026-08-01'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/happyrobot/refs/heads/main/security/happyrobot-trust-center.yml
summary_line: SOC 2 Type II, GDPR, HIPAA, EU AI Act, NIST CSF, DORA
tags:
- AI Agents
- Agent Orchestration
- Voice AI
- Conversational AI
- Logistics
- Freight
- Supply Chain
- Workflow-Automation
- Contact Center
- Telephony
- MCP
- agent-native
- Agent Governance
- Enterprise Automation
trust_url: https://trust.happyrobot.ai/
---
