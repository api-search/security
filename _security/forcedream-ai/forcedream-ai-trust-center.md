---
api_specs:
- filename: forcedream-ai-openapi.yml
  format: yaml
  label: ForceDream API
  slug: forcedream-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/forcedream-ai/refs/heads/main/openapi/forcedream-ai-openapi.yml
certification_count: 3
certifications:
- Cyber Essentials Plus
- UK GDPR
- FCA Consumer Duty (PS22/9)
description: 'A provider-built Trust Centre (not a Vanta/Drata portal) with seven sub-pages. It is unusually candid: the compliance page ticks UK GDPR, Cyber Essentials Plus and FCA Consumer Duty evidence workflows, and marks SOC 2 Type II and ISO/IEC 27001 with a dash and the sentence "ForceDream is not certified" — attributing those to Google Cloud for the London region it runs in. The site footer''s "SOC2 in progress" badge and /v1/capabilities ("soc2":"planned","iso_27001":"planned") agree. The initial keyword probe recorded "SOC 2" from the page text; that is corrected here because the page''s substance is a denial, not a claim.'
kind: trust-center
layout: security
name: Forcedream Ai Trust Center
name_suffix: Trust Center
overview: ForceDream maintains a public trust center documenting Cyber Essentials Plus, UK GDPR, and FCA Consumer Duty (PS22/9) compliance.
provider_name: ForceDream
provider_slug: forcedream-ai
slug: forcedream-ai-trust-center
source_filename: forcedream-ai-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: searched\nprobe: true\nsource: https://www.forcedream.com/trust\nurl: https://www.forcedream.com/trust\nalt_urls:\n  - https://forcedream.ai/trust/\n  - https://www.forcedream.com/trust/compliance\n  - https://www.forcedream.com/trust/controls\n  - https://www.forcedream.com/trust/ledger\n  - https://www.forcedream.com/trust/sla\n  - https://www.forcedream.com/trust/developer\n  - https://www.forcedream.com/trust/enterprise\n  - https://www.forcedream.com/trust/subprocessors\ndescription: >-\n  A provider-built Trust Centre (not a Vanta/Drata portal) with seven sub-pages. It is unusually candid: the\n  compliance page ticks UK GDPR, Cyber Essentials Plus and FCA Consumer Duty evidence workflows, and marks\n  SOC 2 Type II and ISO/IEC 27001 with a dash and the sentence \"ForceDream is not certified\" — attributing\n  those to Google Cloud for the London region it runs in. The site footer's \"SOC2 in progress\" badge and\n  /v1/capabilities (\"\
  soc2\":\"planned\",\"iso_27001\":\"planned\") agree. The initial keyword probe recorded \"SOC 2\"\n  from the page text; that is corrected here because the page's substance is a denial, not a claim.\ncertifications:\n  - name: Cyber Essentials Plus\n    status: claimed\n    evidence: '\"Cyber Essentials+ — UK government-backed cyber security certification.\" (trust/compliance, tick)'\n  - name: UK GDPR\n    status: claimed (compliance statement, not a certification)\n    evidence: '\"UK GDPR — Data residency in eu-west-2 London. DPA available on request.\" (trust/compliance, tick)'\n  - name: FCA Consumer Duty (PS22/9)\n    status: product capability, listed under certifications\n    evidence: '\"Evidence gathering and audit workflows for PS22/9.\" (trust/compliance, tick)'\nexplicitly_not_held:\n  - name: SOC 2 Type II\n    evidence: '\"ForceDream is not SOC 2 certified. Our hosting provider, Google Cloud, is certified for the data centres we run in.\"'\n  - name: ISO/IEC 27001\n    evidence:\
  \ '\"ForceDream is not certified. Google Cloud holds ISO/IEC 27001 for the London region we run in. We would rather say this than let a tick imply otherwise.\"'\nregional_compliance_named: [Nigeria NDPR, Kenya DPA 2019, South Africa POPIA, Singapore PDPA]\nsecurity_controls:\n  encryption: AES-256 at rest; TLS 1.3 in transit; SHA-256 WORM seals\n  access_control: sk_fd_ keys never stored in plaintext, shown once; GitHub/Google OAuth for humans; immediate revocation via POST /v1/account/keys/revoke\n  fraud: 8-signal payout fraud scoring (account age, velocity, IP reputation, amount ratio, device fingerprint, geographic anomaly, hour pattern, recent activity)\n  audit: append-only SHA-256 hash chain, verifiable at GET /v1/ops/worm/verify/:seal; audit export GET /v1/audit/export\n  deployment: '\"Every deployment runs all 69 smoke tests before going live; failed tests trigger automatic rollback\"'\ndata_residency: eu-west-2 London primary; backups eu-west-1; enterprise options London, Dublin,\
  \ Virginia, Singapore\ndpa: '\"DPA — GDPR Article 28. trust@forcedream.ai\" (on request; not published)'\nsubprocessors: https://www.forcedream.com/trust/subprocessors (dated table, 15 May 2026)\ncontacts:\n  trust: trust@forcedream.ai\n  security: security@forcedream.com\n  privacy: privacy@forcedream.com\n  response_commitment: '\"Our trust team responds within one business day.\"'\nevidence:\n  - source: https://www.forcedream.com/trust/compliance\n    http_status: 200\n    fetched: '2026-09-19'\n  - source: https://www.forcedream.com/trust\n    http_status: 200\n    fetched: '2026-09-19'\n  - source: https://api.forcedream.ai/v1/capabilities\n    http_status: 200\n    fetched: '2026-09-19'\n    quote: '\"compliance\":{\"uk_gdpr\":\"compliant\",\"eu_gdpr\":\"compliant\",\"soc2\":\"planned\",\"iso_27001\":\"planned\",\"note\":\"Google Cloud and Vercel hold certifications for the underlying infrastructure. ForceDream holds none of its own.\"}'\ncompliance_pointer_basis: >-\n  type: Compliance\
  \ is emitted on the strength of a published compliance programme (Cyber Essentials Plus\n  claimed, UK GDPR statement, named regional regimes, sub-processor table, security controls page) — not on\n  SOC 2 or ISO 27001, which the provider disclaims.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/forcedream-ai/refs/heads/main/security/forcedream-ai-trust-center.yml
summary_line: Cyber Essentials Plus, UK GDPR, FCA Consumer Duty (PS22/9)
tags:
- AI Agents
- Agent Marketplace
- MCP
- A2A
- Cryptographic Proofs
- AI Inference Routing
- Agent Payments
- Agentic Commerce
- agent-native
- United Kingdom
trust_url: https://www.forcedream.com/trust
---
