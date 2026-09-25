---
api_specs:
- filename: delx-ai-protocol-openapi.json
  format: json
  label: Delx Protocol API
  slug: delx-protocol-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/delx-ai/refs/heads/main/openapi/delx-ai-protocol-openapi.json
- filename: delx-ai-commerce-x402-openapi.json
  format: json
  label: Delx Commerce x402 API
  slug: delx-commerce-x402-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/delx-ai/refs/heads/main/openapi/delx-ai-commerce-x402-openapi.json
certification_count: 0
certifications: []
description: ''
kind: trust-center
layout: security
name: Delx Ai Trust Center
name_suffix: Trust Center
overview: Delx maintains a public trust center covering its security and compliance posture.
provider_name: Delx
provider_slug: delx-ai
slug: delx-ai-trust-center
source_filename: delx-ai-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: searched\nprobe: true\nurl: https://delx.ai/trust\ncertifications: []\nsource: https://delx.ai/trust (200), https://delx.ai/security (200), https://security.delx.ai/ (Delx Security property, 200\n  per the live-properties panel)\nsummary: Delx publishes a trust page built around a five-check evaluation (machine identity, current contract, data and authority,\n  bounded test, evidence and route) and a \"public proof\" list of dated permalinks (independent field review, MCP registry\n  listing, x402 payment manifest, Bazaar coverage matrix, agent card, continuity-audit receipt, incident report, mcp-scorecard\n  results). It states explicitly that none of these is a certification, and the security page adds \"No certification claim\n  - public framework mappings are method inputs; they do not represent a third-party certification.\" There is no SOC 2, ISO\n  27001, PCI DSS, HIPAA or FedRAMP claim anywhere, so no Compliance pointer is emitted.\n\
  evidence:\n- source: https://delx.ai/trust\n  http_status: 200\n  fetched: '2026-09-19'\n  keywords:\n  - trust\n  - security.txt\n  - evidence\n  - bounded test\n  - not a certification\n- source: https://delx.ai/security\n  http_status: 200\n  fetched: '2026-09-19'\n  keywords:\n  - defensive assurance\n  - No certification claim\n  - security.txt\n  - disclosure policy\npublic_proof_links_declared:\n- Would Pay Again, issue 5 (2026-08-11) independent field review of a tested subset of Commerce calls\n- Official MCP Registry listing io.github.davidmosiah/delx-mcp-a2a (2026-08-06)\n- Live x402 payment manifest (2026-08-26)\n- Coinbase Bazaar index coverage matrix (2026-08-07)\n- A2A agent card / ERC-8004 discovery surface (2026-08-26)\n- Continuity audit live receipt (2026-08-26)\n- Protocol write-outage incident report (2026-08-17)\n- mcp-scorecard results for delx-living-body and astral-mcp (2026-08-24)\nnote: The probe-security-programs.py keyword threshold did not fire on this page\
  \ (it looks for compliance-certification vocabulary);\n  recorded by hand because the page is a real trust surface whose whole point is the absence of badges.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/delx-ai/refs/heads/main/security/delx-ai-trust-center.yml
summary_line: trust center published
tags:
- Agents
- AI Agents
- MCP
- A2A
- x402
- Agentic Commerce
- Agent Continuity
- Agent Recovery
- Media Generation
- Web Intelligence
- Data Quality
- Agent-Native
trust_url: https://delx.ai/trust
---
