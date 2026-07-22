---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: tagomi.com
  spf: true
hosts:
- cert_expires: Aug 28 21:57:47 2026 GMT
  host: tagomi.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Tagomi Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Tagomi, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Tagomi
provider_slug: tagomi
slug: tagomi-domain-security
source_filename: tagomi-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: tagomi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 28 21:57:47 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: tagomi.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tagomi/refs/heads/main/security/tagomi-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Crypto
- Cryptocurrency
- Prime Brokerage
- Institutional Trading
- Digital Assets
- Trading
- Acquired
---
