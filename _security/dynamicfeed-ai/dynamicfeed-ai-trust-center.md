---
api_specs:
- filename: dynamicfeed-ai-openapi.yml
  format: yaml
  label: Dynamic Feed REST API
  slug: dynamic-feed-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dynamicfeed-ai/refs/heads/main/openapi/dynamicfeed-ai-openapi.yml
certification_count: 0
certifications: []
description: ''
kind: trust-center
layout: security
name: Dynamicfeed Ai Trust Center
name_suffix: Trust Center
overview: Dynamic Feed maintains a public trust center covering its security and compliance posture.
provider_name: Dynamic Feed
provider_slug: dynamicfeed-ai
slug: dynamicfeed-ai-trust-center
source_filename: dynamicfeed-ai-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: searched\nprobe: true\nsource: https://dynamicfeed.ai/trust (HTTP 200, read in full 2026-09-19) and https://dynamicfeed.ai/enterprise\nurl: https://dynamicfeed.ai/trust\nname: Trust Center — \"verify everything about us\"\ncertifications: []\ncertifications_note: 'NONE HELD. probe-security-programs.py matched the keyword \"SOC 2\" on this page and recorded\n  it as a certification; the page actually says the opposite: \"soc 2 · dpa — On request. SOC 2 and a signed DPA\n  are pursued against a signed enterprise requirement, not claimed speculatively. We hold no certification we haven''t\n  earned.\" That line is corrected here so the artifact does not credit a certification the provider explicitly disclaims.\n  No Compliance pointer is emitted.'\nposture_stated:\n- area: transport\n  claim: TLS everywhere; Content-Security-Policy enforced site-wide\n  verified: probed — TLSv1.3, HSTS max-age 63072000 preload, CSP header observed (security/dynamicfeed-ai-domain-security.yml)\n\
  - area: data boundary\n  claim: No personal data required to read; no prompts or queries stored; nothing sold or shared; read-only by design\n- area: audit trail\n  claim: Ed25519 over canonical bytes; fingerprints time-stamped by an independent RFC 3161 authority; append-only\n    Merkle transparency log\n- area: provenance\n  claim: Source, licence and freshness attached to every value; full catalog at /sources\n- area: sso / rbac\n  claim: NOT live yet; available on an enterprise contract\n  status: roadmap\n- area: soc 2 / dpa\n  claim: On request, pursued against a signed enterprise requirement; not claimed\n  status: not held\n- area: uptime\n  claim: Live status and measured uptime at /uptime and /ops; a formal SLA is part of an enterprise agreement\n  status: no SLA\ncontact: hello@dynamicfeed.ai (data-handling questions or a DPA)\nrelated:\n  security_advisories: https://dynamicfeed.ai/security/advisories\n  signing_key_registry: https://dynamicfeed.ai/.well-known/signing-key-registry.json\n\
  \  verification_standard: https://dynamicfeed.ai/standard\n  status: https://dynamicfeed.ai/uptime\nevidence:\n- source: https://dynamicfeed.ai/trust\n  status: 200\n  quote: We hold no certification we haven't earned.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dynamicfeed-ai/refs/heads/main/security/dynamicfeed-ai-trust-center.yml
summary_line: trust center published
tags:
- Live Data
- AI Agents
- MCP
- A2A
- Agent-Native
- Provenance
- Weather
- Natural Hazards
- Vulnerabilities
- Sanctions
- Space
- Robotics
- x402
- Receipts
- Notary
- Australia
trust_url: https://dynamicfeed.ai/trust
---
