---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: effectiv.ai
  spf: true
hosts:
- host: effectiv.ai
  https: false
kind: domain-security
layout: security
method: probed
name: Effectiv Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Effectiv, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Effectiv
provider_slug: effectiv
slug: effectiv-domain-security
source_filename: effectiv-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: effectiv.ai\n  https: false\ndomains:\n- domain: effectiv.ai\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/effectiv/refs/heads/main/security/effectiv-domain-security.yml
summary_line: DNSSEC · DMARC
tags:
- Company
- Security
- Fraud Detection
- Risk
- Decisioning
- Identity Verification
- KYC
- KYB
- AML
- Transaction Monitoring
- Fintech
- Device Intelligence
---
