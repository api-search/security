---
api_specs:
- filename: thehiveryiq-com-hivemorph-openapi.yml
  format: yaml
  label: Hive Receipts and Agent Commerce API (HiveMorph)
  slug: hivemorph-receipts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thehiveryiq-com/refs/heads/main/openapi/thehiveryiq-com-hivemorph-openapi.yml
- filename: thehiveryiq-com-hivecompute-openapi.yml
  format: yaml
  label: HiveCompute Inference Router API
  slug: hivecompute-inference-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thehiveryiq-com/refs/heads/main/openapi/thehiveryiq-com-hivecompute-openapi.yml
certification_count: 0
certifications: []
description: ''
kind: trust-center
layout: security
name: Thehiveryiq Com Trust Center
name_suffix: Trust Center
overview: Hive Civilization maintains a public trust center covering its security and compliance posture.
provider_name: Hive Civilization
provider_slug: thehiveryiq-com
slug: thehiveryiq-com-trust-center
source_filename: thehiveryiq-com-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: searched\nprobe: true\nsource: https://thehiveryiq.com/security/\nurl: https://thehiveryiq.com/security/\npages:\n- https://thehiveryiq.com/security/\n- https://thehiveryiq.com/security/soc2-self-attested/\n- https://thehiveryiq.com/security/iso-27001-self-attested/\n- https://thehiveryiq.com/security/founder-risk/\n- https://thehiveryiq.com/compliance/\n- https://thehiveryiq.com/trust\n- https://thehiveryiq.com/security/policy-evidence-2026-09-05.json\ncertifications: []\nself_attestations:\n- framework: SOC 2 (AICPA TSC 2017)\n  url: https://thehiveryiq.com/security/soc2-self-attested/\n  status: self-attested review inventory; \"No independent SOC 2 report or executed engagement letter was supplied\n    in this review.\"\n- framework: ISO/IEC 27001:2022\n  url: https://thehiveryiq.com/security/iso-27001-self-attested/\n  status: self-attested review inventory of 93 Annex A control topics; \"not an ISO certificate or independent audit\".\n\
  - framework: HIVECOMPLY control dashboard\n  url: https://thehiveryiq.com/compliance/\n  status: self-scored 96.2/100 across 158 controls and 12 frameworks (SOC 2, ISO 27001/27017/27018/27701/27036/42001,\n    GDPR, eIDAS 2.0, NIS2, DORA; EU AI Act pending), \"Machine = automated; Self = operator-attested\". Last scanned\n    2026-05-08.\ncorrection: 'The automated probe (probe-security-programs.py) keyword-matched ''SOC 2'', ''ISO 27001'', ''FedRAMP''\n  and ''GDPR'' on /security and wrote them as certifications. Read in context, the page says the opposite: ''No\n  executed SOC 2 engagement letter, independent audit report or ISO certificate was supplied for this review'';\n  ''Audit Engagement: Not verified. AICPA SOC 2 Report: Not supplied. ISO 27001: Date unapproved''; ''No independent\n  penetration-test agreement or report was supplied''. FedRAMP appears only as a framework name in the HiveComply\n  product list. certifications is therefore EMPTY. What Hive does publish, unusually,\
  \ is a dated, source-referenced\n  evidence review of its own posture, including the gaps.'\nposture_highlights:\n  review_date: '2026-09-05'\n  hosting: Four Render services in Oregon, United States; Cloudflare edge; static distribution global\n  cryptography: Ed25519 in application processes (no verified KMS boundary); ML-DSA-65 signer service; algorithm\n    labels are not validation certificates\n  key_person_risk: Single-founder operation disclosed at /security/founder-risk/; treasury 0x15184Bf5...436E on\n    Base; proposed 2-of-3 Safe not deployed\n  penetration_testing: No independent test report supplied\n  subprocessors: Render, Cloudflare, Stripe (not verified active), Mercury (not verified), GitHub, Supabase/other\n    storage (not verified)\n  machine_readable_evidence: https://thehiveryiq.com/security/policy-evidence-2026-09-05.json (deployments, signing_custody_matrix,\n    retention_inventory, claims_registry, change_log)\nevidence:\n- source: https://thehiveryiq.com/security/\n\
  \  http_status: 200\n  fetched: '2026-09-19'\n  quote: No executed SOC 2 engagement letter, independent audit report or ISO certificate was supplied for this\n    review.\n- source: https://thehiveryiq.com/security/soc2-self-attested/\n  http_status: 200\n  fetched: '2026-09-19'\n  quote: 'Self-attestation notice: not a SOC 2 report.'\n- source: https://thehiveryiq.com/security/iso-27001-self-attested/\n  http_status: 200\n  fetched: '2026-09-19'\n  quote: This is a self-maintained review inventory, not an ISO certificate or independent audit.\n- source: https://thehiveryiq.com/compliance/\n  http_status: 200\n  fetched: '2026-09-19'\n  quote: 96.2 / 100 Overall compliance score ... Machine = automated; Self = operator-attested.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/thehiveryiq-com/refs/heads/main/security/thehiveryiq-com-trust-center.yml
summary_line: trust center published
tags:
- Agents
- Agentic Commerce
- A2A
- MCP
- x402
- Receipts
- Digital Signature
- Post-Quantum Cryptography
- Attestation
- Decentralized Identity
- Stablecoins
- Inference
- LLM Routing
- Compliance
- agent-native
- United States
trust_url: https://thehiveryiq.com/security/
---
