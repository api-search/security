---
api_specs:
- filename: scvd-store-openapi.json
  format: json
  label: SCVD General Store API
  slug: scvd-general-store-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scvd-store/refs/heads/main/openapi/scvd-store-openapi.json
certification_count: 0
certifications: []
description: ''
kind: trust-center
layout: security
name: Scvd Store Trust Center
name_suffix: Trust Center
overview: Record Creative Co. LLC maintains a public trust center covering its security and compliance posture.
provider_name: Record Creative Co. LLC
provider_slug: scvd-store
slug: scvd-store-trust-center
source_filename: scvd-store-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: searched\nprobe: true\nurl: https://scvd.store/trust\nmachine_readable: https://scvd.store/.well-known/trust.json\nfile: ../well-known/scvd-store-trust.json\ncertifications: []\nsummary: 'A trust surface built for automated diligence rather than a certification showcase: /.well-known/trust.json\n  (the security.txt Policy target, 93 KB) and its human twin /trust name the operator (Record Creative Co. LLC,\n  Oak City, North Carolina; kind individual), the standards implemented end to end, wallet-safety mechanisms, data\n  handling (no cookies, no IP logs, no accounts), the refund policy, external registry records with dates, and —\n  unusually — an explicit not_claimed list. No SOC 2, ISO 27001, PCI DSS, HIPAA or any third-party audit is claimed,\n  so no Compliance pointer is emitted; the TrustCenter pointer records that the surface exists and says what it\n  says.'\nnot_claimed:\n- No third-party security audit of anything here, and no plans\
  \ for one.\n- No VAT number and no D-U-N-S. There IS a registered company — Record Creative Co. LLC.\n- No escrow and no chargebacks.\n- No insurance, no bonding, no regulator, and nothing here is offered as a financial service.\n- One ed25519 signing key and one operator — \"the wrong root of trust for compliance, dispute resolution, or anything\n  load-bearing\".\n- No post-quantum signatures.\n- No reputation score on any actor, ours or anybody's, ever, and no ranking of one host against another.\n- No independent audit of the books.\nindependently_checkable:\n  signatures: GET /api/verify/{id} + key history at /.well-known/scvd-signing-key\n  settlement: every certificate binds settlement_tx, checkable on the chain explorer\n  key_history: /.well-known/anchor-log.json, OTS-anchored into Bitcoin\n  ecosystem_record: corpus.json, hash-chained and OTS-stamped\nexternal_records:\n- registry: UCP Checker\n  url: https://ucpchecker.com/check/scvd.store\n  confirmed: '2026-09-19'\n- registry:\
  \ MPPScan\n  url: https://www.mppscan.com/server/d58b4c8d9dc872c8308b594e4b4117bff2255f83b47f054e492b2a2fbc0ddb7b\n  confirmed: '2026-09-19'\n- registry: HOL awesome-ai-plugins\n  url: https://github.com/hashgraph-online/awesome-ai-plugins#tools--integrations\n  confirmed: '2026-09-19'\n- registry: A2A Registry\n  url: https://a2aregistry.org/api/agents/3ec62f32-4e67-4382-8d15-2b6bf689f33a\n  confirmed: '2026-09-18'\nevidence:\n- source: https://scvd.store/.well-known/trust.json\n  http_status: 200\n  keywords:\n  - trust\n  - independence\n  - operator\n  - standards\n  - data_handling\n  - not_claimed\n  - refund_policy\n- source: https://scvd.store/trust\n  http_status: 200\n  content_type: application/json\n- source: https://scvd.store/.well-known/security.txt\n  http_status: 200\n  note: 'Policy: line points at trust.json'\nnote: probe-security-programs.py recorded trust=none because it requires named certifications; this artifact is\n  written by hand from the pages above and claims\
  \ none.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/scvd-store/refs/heads/main/security/scvd-store-trust-center.yml
summary_line: trust center published
tags:
- Agents
- Agentic Commerce
- x402
- Payments
- Micropayments
- Stablecoins
- USDC
- Verification
- Conformance
- Attestation
- Observability
- MCP
- A2A
- Universal Commerce Protocol
- Signatures
- agent-native
- United States
trust_url: https://scvd.store/trust
---
