---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: sea.com
  spf: true
hosts:
- cert_expires: Sep 22 11:02:14 2026 GMT
  host: www.sea.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Sea Group Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Sea Group (Sea Limited), probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Sea Group (Sea Limited)
provider_slug: sea-group
slug: sea-group-domain-security
source_filename: sea-group-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.sea.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 22 11:02:14 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: sea.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sea-group/refs/heads/main/security/sea-group-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Holding Company
- Southeast Asia
- E-commerce
- Digital Entertainment
- Financial Services
- Shopee
- Garena
- SeaMoney
---
