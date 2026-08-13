---
api_specs:
- filename: lily-ai-lilyapp-api-openapi.yml
  format: yaml
  label: LilyApp Middleware API
  slug: lilyapp-middleware-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lily-ai/refs/heads/main/openapi/lily-ai-lilyapp-api-openapi.yml
certifications: []
description: ''
kind: trust-center
layout: security
name: Lily Ai Trust Center
name_suffix: Trust Center
overview: Lily AI maintains a public trust center covering its security and compliance posture.
provider_name: Lily AI
provider_slug: lily-ai
slug: lily-ai-trust-center
source_filename: lily-ai-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: probed\nsource: >-\n  DNS resolution of trust.lily.ai and live HTTPS probes (2026-08-12), plus\n  https://www.lily.ai/security\ntrust_center:\n  url: https://trust.lily.ai/\n  exists: true\n  platform: Drata\n  platform_evidence: 'DNS CNAME trust.lily.ai -> trust.cname.drata.com'\n  readable: false\n  http_status: 403\n  block_reason: >-\n    Cloudflare managed bot challenge. Every automated request — including\n    /.well-known/security.txt and the Drata API paths — returns HTTP 403 with the\n    \"Just a moment...\" interstitial (cf challenge, zone trust.lily.ai). A human with\n    a JavaScript-capable browser can read the page; a machine cannot.\ncertifications: []\ncertifications_note: >-\n  NO certification is recorded, because none could be verified. A Drata-backed trust\n  center is where a SOC 2 Type II or ISO 27001 attestation would normally be\n  published, but the challenge page prevents reading it, and Lily AI's public\n  security\
  \ page (https://www.lily.ai/security) names no certification at all — it\n  states only that the company \"aligns with industry standards and customer\n  requirements\". Per the no-fabrication rule, presence of a Drata tenant is NOT\n  treated as evidence of any specific certification, and no `Compliance` pointer is\n  emitted.\npublic_security_claims:\n  source: https://www.lily.ai/security\n  claims:\n  - Encryption in transit and at rest\n  - Least-privilege access\n  - Secrets kept server-side\n  - Inputs validated\n  - Access logged\n  - Customer data used only to operate the customer's campaigns, never sold\nx-evidence:\n- url: https://trust.lily.ai/\n  status: 403\n  fetched: '2026-08-12'\n- url: https://trust.lily.ai/.well-known/security.txt\n  status: 403\n  fetched: '2026-08-12'\n- url: https://www.lily.ai/security\n  status: 200\n  fetched: '2026-08-12'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lily-ai/refs/heads/main/security/lily-ai-trust-center.yml
summary_line: trust center published
tags:
- Company
- Retail
- E-Commerce
- Artificial Intelligence
- Product Data
- Advertising
- Agentic Commerce
- Search
- Marketing
trust_url: ''
---
