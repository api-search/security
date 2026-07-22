---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: zeal.app
  spf: true
hosts:
- cert_expires: Aug 22 12:39:52 2026 GMT
  host: www.zeal.app
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Zeal Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Zeal, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Zeal
provider_slug: zeal
slug: zeal-domain-security
source_filename: zeal-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.zeal.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 22 12:39:52 2026 GMT\n  hsts: false\ndomains:\n- domain: zeal.app\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zeal/refs/heads/main/security/zeal-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Infra Devtools
- Cryptocurrency
- Wallet
- DeFi
- Payments
- Web3
- Stablecoins
---
