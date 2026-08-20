---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: acinq.co
  spf: true
hosts:
- cert_expires: Oct 29 11:14:46 2026 GMT
  host: acinq.co
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 29 11:14:46 2026 GMT
  host: phoenix.acinq.co
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Acinq Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Acinq, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Acinq
provider_slug: acinq
slug: acinq-domain-security
source_filename: acinq-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: acinq.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 29 11:14:46 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: phoenix.acinq.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 29 11:14:46 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: acinq.co\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/acinq/refs/heads/main/security/acinq-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Blockchain
- Bitcoin
- Lightning Network
- Payments
- Open-Source
- Self-Custody
- Node Software
- Cryptocurrency
- Developer Tools
---
