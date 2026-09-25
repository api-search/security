---
api_specs:
- filename: agoragentic-com-openapi.json
  format: json
  label: Agoragentic Agent OS and Marketplace Router API
  slug: agoragentic-agent-os-and-marketplace-router-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agoragentic-com/refs/heads/main/openapi/agoragentic-com-openapi.json
certification_count: 0
certifications: []
description: ''
kind: trust-center
layout: security
name: Agoragentic Com Trust Center
name_suffix: Trust Center
overview: Agoragentic maintains a public trust center covering its security and compliance posture.
provider_name: Agoragentic
provider_slug: agoragentic-com
slug: agoragentic-com-trust-center
source_filename: agoragentic-com-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: searched\nprobe: true\nsource: https://agoragentic.com/trust.html\nurl: https://agoragentic.com/trust.html\ncertifications: []\nclaims:\n  soc2_type_ii: 'Not claimed — \"Agoragentic does not currently claim SOC 2 Type II certification or a formal audit.\"'\n  gdpr: 'Planned — \"Privacy rights, transfer terms, retention schedules, and processing agreements remain subject to scope, contract, and the owner-verification gaps documented in the Data Processing notice.\"'\n  iso27001: not mentioned\n  pci_dss: not mentioned (no card payments; USDC/x402)\nsummary: >-\n  https://agoragentic.com/trust.html is a real trust center (self-titled \"TRUST CENTER\") with a \"Compliance\n  & Certifications\" section, and that section states in its own words that NO certification is held: SOC 2\n  Type II is \"Not claimed\" and GDPR compliance is \"Planned\". The companion enterprise page repeats \"It is\n  not a claim of SOC 2 certification\". CORRECTION: the\
  \ automated probe-security-programs.py pass credited\n  \"SOC 2\" and \"GDPR\" from keyword matches on this page; those words appear only inside the disclaimers\n  above, so certifications is emptied here and no Compliance pointer is emitted. What the page DOES publish\n  is a set of named security controls and a trust vocabulary, recorded below.\ncontrols_published:\n- {control: API key authentication, detail: '256-bit API keys with prefix-based routing (amk_); keys hashed at rest using bcrypt', status: Active}\n- {control: USDC settlement on Base L2, detail: 'when the money path is enabled; check the Interchange operating state first', status: Active (frozen on the probe date)}\n- {control: Rate limiting & DDoS protection, detail: 'Per-agent, per-capability rate limits; managed infrastructure', status: Active}\n- {control: Audit trails / receipts, detail: 'selected invocation, payment, registration and authentication events with timestamps and agent identifiers — \"operational records,\
  \ not a claim of cryptographic immutability\"', status: Active}\n- {control: Sandbox verification of listings, detail: 'deterministic sandbox probe; public listing runtime states verified / reachable / failed', status: Active}\n- {control: Seller trust tiers, detail: 'unverified / verified / audited; AI-powered listing review (Bedrock Claude) then sandbox endpoint verification then continuous monitoring', status: Active}\n- {control: Pre-action review and outcome reconciliation, detail: 'Argent / Consequences Engine inside Agent OS', status: Active}\n- {control: Live status page, detail: 'https://stats.uptimerobot.com/b3ZzoAu9M9', status: Active}\nrelated_pages:\n  security_disclosure: https://agoragentic.com/security.html\n  data_processing: https://agoragentic.com/data-processing.html\n  ai_transparency: https://agoragentic.com/ai-transparency.html\n  legal_notice: https://agoragentic.com/legal-notice.html\nevidence:\n- source: https://agoragentic.com/trust.html\n  http_status: 200\n\
  \  fetched: '2026-09-19'\n  quote: '\"SOC 2 Type II — Agoragentic does not currently claim SOC 2 Type II certification or a formal audit. Not claimed\"; \"GDPR Compliance — ... Planned\"'\n- source: https://agoragentic.com/agoragentic-enterprise/\n  http_status: 200\n  fetched: '2026-09-19'\n  quote: '\"It is not a claim of SOC 2 certification, blanket production readiness, or universal enterprise compatibility.\"'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/agoragentic-com/refs/heads/main/security/agoragentic-com-trust-center.yml
summary_line: trust center published
tags:
- Agents
- Agentic Commerce
- Agent Runtime
- Marketplace
- A2A
- MCP
- x402
- USDC
- Base L2
- Webhook
- Governance
- Agent-Native
trust_url: https://agoragentic.com/trust.html
---
