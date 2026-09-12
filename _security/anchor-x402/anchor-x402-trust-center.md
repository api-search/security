---
api_specs:
- filename: anchor-x402-openapi.json
  format: json
  label: anchor-x402 API
  slug: anchor-x402-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anchor-x402/refs/heads/main/openapi/anchor-x402-openapi.json
certification_count: 0
certifications: []
description: ''
kind: trust-center
layout: security
name: Anchor X402 Trust Center
name_suffix: Trust Center
overview: anchor-x402 maintains a public trust center covering its security and compliance posture.
provider_name: anchor-x402
provider_slug: anchor-x402
slug: anchor-x402-trust-center
source_filename: anchor-x402-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-09-11'\nmethod: searched\nprobe: true\nsource: https://anchor-x402.com/trust/\nurl: https://anchor-x402.com/trust/\nhttp_status: 200\ntrust_center_present: true\ncertifications: []\ncertification_count: 0\ncertifications_explicitly_disclaimed:\n- SOC 2\n- ISO 27001\n- PCI DSS\n- HIPAA\n- GDPR DPA\nx-correction: >-\n  0-working/probe-security-programs.py wrote this file on 2026-09-11 with certifications [SOC 2, ISO 27001,\n  HIPAA, GDPR] from a bare keyword match on the trust-portal page. Every one of those matches is a NEGATION.\n  The page's own words are \"We do not hold SOC 2, ISO 27001, or PCI certifications\" and \"No SOC 2 / ISO\n  27001 / PCI / HIPAA certification. Roadmap items, not blockers for the commodity tier.\" The list was\n  corrected to empty by hand and no Compliance pointer was emitted. A scorer reading the generated file\n  would have credited this provider with four certifications it goes out of its way to say it does not hold.\nposture:\
  \ >-\n  The trust portal is unusually substantial for an uncertified provider and is built around an explicit\n  argument: publish the reasoning instead of the certificates. It carries six documents totalling roughly\n  22,000 words - a STRIDE-lite per-service threat model, a pre-filled SIG-Lite vendor security\n  questionnaire, a code-level self-audit guide mapping 15 compliance concerns to file and line ranges in the\n  MIT-licensed source, a regulated-deployment guide covering trust boundaries and AWS compliance\n  inheritance, an on-chain verifiability primer with live mainnet hashes, and observability docs.\ndocuments:\n- name: Threat model\n  url: https://anchor-x402.com/trust/threat-model.html\n  status: 200\n  form: STRIDE-lite per-service enumeration with mitigations and residual risk\n  approx_words: 5400\n- name: Security questionnaire\n  url: https://anchor-x402.com/trust/security-questionnaire.html\n  status: 200\n  form: Pre-filled SIG-Lite-style vendor security response\
  \ across 11 sections\n  approx_words: 4300\n- name: Self-audit guide\n  url: https://anchor-x402.com/trust/self-audit.html\n  form: 15 compliance concerns mapped to specific files and line ranges in the codebase\n  approx_words: 4600\n- name: Regulated deployment guide\n  url: https://anchor-x402.com/trust/regulated-deployment.html\n  form: Trust boundaries, AWS compliance inheritance, customer-side responsibilities\n  approx_words: 5300\n- name: On-chain verifiability\n  url: https://anchor-x402.com/trust/on-chain-verifiability\n  status: 200\n  form: The cryptographic primitive and how a customer verifies anchors without contacting the service\n  approx_words: 1800\n- name: Observability\n  url: https://anchor-x402.com/trust/observability.html\n  form: CloudWatch dashboard and status-page setup, what to expose, what consumers should monitor\n  approx_words: 1000\ncompensating_controls_claimed:\n- MIT-licensed open-source codebase, auditable line by line\n- On-chain verifiability - anchors\
  \ are readable from Base and Solana mainnet independently of the service\n- Deliberately stateless architecture with no per-customer PII at rest\n- Compliance inheritance from AWS infrastructure (Lambda, Secrets Manager, CloudWatch)\ndisclosed_gaps:\n- No SOC 2, ISO 27001, PCI-DSS, HIPAA certification - stated as roadmap items, not blockers for the commodity tier\n- No cyber liability or tech E&O insurance - to be obtained when first contractually required\n- No formal written incident-response runbook - a disclosure email exists, the runbook is on the roadmap\n- No DPA template at the commodity tier\nscope_limitation_published: >-\n  The threat model covers thirteen trust-relevant endpoints. The five LLM content endpoints (roast, oracle,\n  tldr, aura, grade) are documented as explicitly out of scope - freeform text in, generated content out,\n  no wallet-risk verdict and no compliance evidence.\ninstitutional_tier:\n  status: available on request\n  price: USD 499-5,000+/mo\n  inclusions:\n\
  \  - per-tenant authentication\n  - signed MSA/DPA/SLA\n  - WORM evidence vault on S3 Object Lock\n  - GDPR Article 17 erasure reconciled with AML retention\n  contact: hello@anchor-x402.com\nstatus_page: https://anchor-x402.betteruptime.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/anchor-x402/refs/heads/main/security/anchor-x402-trust-center.yml
summary_line: trust center published
tags:
- Company
- x402
- Agents
- Payments
- Blockchain
- MCP
- Web3
- Pay Per Call
- Agent Payments
- Stablecoins
- Compliance
- Attestation
trust_url: https://anchor-x402.com/trust/
---
