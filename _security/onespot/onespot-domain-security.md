---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: onespot.com
  spf: true
hosts:
- cert_expires: Dec  2 23:59:59 2026 GMT
  host: onespot.com
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Onespot Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for OneSpot, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: OneSpot
provider_slug: onespot
slug: onespot-domain-security
source_filename: onespot-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: onespot.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec  2 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: onespot.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/onespot/refs/heads/main/security/onespot-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- Company
- AdTech
- Content Marketing
- Marketing Technology
- Personalization
- Advertising
- Machine-Learning
- Austin
---
