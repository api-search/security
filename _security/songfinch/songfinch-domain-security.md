---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: songfinch.com
  spf: true
hosts:
- cert_expires: Nov 14 22:49:14 2026 GMT
  host: www.songfinch.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Songfinch Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Songfinch, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Songfinch
provider_slug: songfinch
slug: songfinch-domain-security
source_filename: songfinch-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.songfinch.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 14 22:49:14 2026 GMT\n  hsts: false\ndomains:\n- domain: songfinch.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/songfinch/refs/heads/main/security/songfinch-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Music
- Marketplace
- E-Commerce
- Gifting
- Consumer
- Entertainment
- Creator Economy
- Personalization
---
