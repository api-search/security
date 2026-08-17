---
api_specs:
- filename: seamless-ai-public-api-openapi-original.json
  format: json
  label: Seamless.AI Public API
  slug: seamless-ai-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/seamless-ai/refs/heads/main/openapi/_original/seamless-ai-public-api-openapi-original.json
- filename: seamless-ai-mcp-server-openapi-original.yaml
  format: yaml
  label: Seamless.AI MCP Server
  slug: seamless-ai-mcp-server
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/seamless-ai/refs/heads/main/openapi/_original/seamless-ai-mcp-server-openapi-original.yaml
certifications: []
description: ''
kind: trust-center
layout: security
name: Seamless Ai Trust Center
name_suffix: Trust Center
overview: Seamless.AI maintains a public trust center covering its security and compliance posture.
provider_name: Seamless.AI
provider_slug: seamless-ai
slug: seamless-ai-trust-center
source_filename: seamless-ai-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-14'\nmethod: probed\nprobe: true\nurl: https://trust.seamless.ai/\nplatform: Vanta\nconfirmed: true\nhttp_status: 200\nsubpages:\n  - {path: /controls, status: 200}\n  - {path: /faq, status: 200}\n  - {path: /resources, status: 200}\ncertifications: []\ncertifications_readable: false\nnote: >-\n  Seamless.AI publishes a Vanta-hosted trust center at trust.seamless.ai. The host, its /controls,\n  /faq and /resources routes all return HTTP 200 and the served HTML identifies Vanta as the\n  platform with `<link rel=\"canonical\" href=\"https://trust.seamless.ai\">` and the title \"Seamless\n  Trust Center\". The certification list, control set and document library render entirely\n  client-side from a JavaScript bundle, and Vanta exposes no anonymous JSON endpoint on this\n  host (every /api/* path returns the same SPA shell at 200). We therefore confirm the trust\n  center EXISTS but assert NO individual certification: `certifications` is deliberately empty\n\
  \  rather than filled in from third-party summaries. Access to the underlying reports is typically\n  request-gated behind an NDA on Vanta trust centers.\nrecheck: >-\n  A future run should retry with a JS-capable fetch, or ask the provider for the Vanta trust\n  center's public share link, before recording SOC 2 / ISO 27001 / ISO 27701 as verified.\nsecurity_txt: false\nsecurity_txt_note: /.well-known/security.txt returns 404 or 403 on all five Seamless.AI hosts probed.\nvulnerability_disclosure_program: false\nvulnerability_disclosure_note: >-\n  No bug bounty (HackerOne / Bugcrowd / Intigriti), no responsible-disclosure page and no\n  security@ address were found. Probed seamless.ai/security, /trust, /responsible-disclosure,\n  /policies/security and /security-and-compliance — all 404. The only published contact addresses\n  are privacy@seamlessleads.com (privacy policy), sales@seamlessleads.com and\n  devs@seamlesscontacts.com. Because nothing was verified, no VulnerabilityDisclosure\
  \ and no\n  Security pointer is emitted.\nprivacy_posture:\n  privacy_policy: https://seamless.ai/policies/privacy-policy\n  terms_of_use: https://seamless.ai/policies/terms-of-use\n  gdpr: >-\n    The privacy policy states Seamless.AI transfers personal data using European Commission\n    standard contractual clauses for transfers outside the EU/EEA, Switzerland and the UK.\n  privacy_contact: privacy@seamlessleads.com\n  note: >-\n    Seamless.AI is a B2B contact-data broker. Data-protection posture is a first-order concern for\n    any integrator of this API, which is why the unreadable certification list is worth flagging\n    rather than glossing.\nevidence:\n  - {source: 'https://trust.seamless.ai/', http_status: 200, fetched: '2026-08-14', keywords: [trust center, vanta]}\n  - {source: 'https://trust.seamless.ai/controls', http_status: 200, fetched: '2026-08-14'}\n  - {source: 'https://seamless.ai/security', http_status: 404, fetched: '2026-08-14'}\n  - {source: 'https://seamless.ai/.well-known/security.txt',\
  \ http_status: 404, fetched: '2026-08-14'}\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/seamless-ai/refs/heads/main/security/seamless-ai-trust-center.yml
summary_line: trust center published
tags:
- B2B
- Contact Data
- Sales Intelligence
- Prospecting
- Lead Generation
- CRM Enrichment
- Data Enrichment
- MCP
- Agents
- Sales Automation
trust_url: https://trust.seamless.ai/
---
