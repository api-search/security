---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: violet.co
  spf: true
hosts:
- cert_expires: Aug 20 20:57:23 2026 GMT
  host: www.violet.co
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- host: app.violet.co
  https: false
kind: domain-security
layout: security
method: probed
name: Violet Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Violet, probed live across 2 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Violet
provider_slug: violet
slug: violet-domain-security
source_filename: violet-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.violet.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 20 20:57:23 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: app.violet.co\n  https: false\ndomains:\n- domain: violet.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/violet/refs/heads/main/security/violet-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Compliance
- Identity
- DeFi
- Blockchain
- KYC
- AML
- Web3
- Decentralized Identity
- Sanctions Screening
- OAuth
---
