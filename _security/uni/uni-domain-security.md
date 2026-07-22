---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: uni.cards
  spf: true
hosts:
- cert_expires: Aug 22 17:59:27 2026 GMT
  host: www.uni.cards
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Uni Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Uni, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Uni
provider_slug: uni
slug: uni-domain-security
source_filename: uni-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.uni.cards\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 22 17:59:27 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\ndomains:\n- domain: uni.cards\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/uni/refs/heads/main/security/uni-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- FinTech
- Credit
- Credit Cards
- Consumer Finance
- Payments
- India
---
