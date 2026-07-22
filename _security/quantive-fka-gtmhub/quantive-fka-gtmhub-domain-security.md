---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: quantive.com
  spf: true
hosts:
- cert_expires: Sep 25 17:37:14 2026 GMT
  host: quantive.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Quantive Fka Gtmhub Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Quantive (fka Gtmhub), probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Quantive (fka Gtmhub)
provider_slug: quantive-fka-gtmhub
slug: quantive-fka-gtmhub-domain-security
source_filename: quantive-fka-gtmhub-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: quantive.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 17:37:14 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: quantive.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/quantive-fka-gtmhub/refs/heads/main/security/quantive-fka-gtmhub-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- OKR
- Strategy Execution
- Goal Management
- Performance Management
- SaaS
- Extensibility SDK
- CLI
---
