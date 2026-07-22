---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: gloset.mx
  spf: true
hosts:
- cert_expires: Sep 17 23:59:59 2026 GMT
  host: gloset.mx
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Gloset Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Gloset, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Gloset
provider_slug: gloset
slug: gloset-domain-security
source_filename: gloset-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: gloset.mx\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 17 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: gloset.mx\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gloset/refs/heads/main/security/gloset-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Company
- Marketplace
- Fashion
- E-Commerce
- Resale
- Peer-to-Peer
- Mexico
- Retail
---
