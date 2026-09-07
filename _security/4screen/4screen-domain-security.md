---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: 4screen.com
  spf: true
hosts:
- cert_expires: Nov  3 10:11:24 2026 GMT
  host: 4screen.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 28 17:56:06 2026 GMT
  host: api.4screen.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: 4Screen Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for 4.screen, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: 4.screen
provider_slug: 4screen
slug: 4screen-domain-security
source_filename: 4screen-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: 4screen.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  3 10:11:24 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.4screen.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 28 17:56:06 2026 GMT\n  hsts: null\ndomains:\n- domain: 4screen.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/4screen/refs/heads/main/security/4screen-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Advertising
- AdTech
- Automotive
- Mobility
- Connected Vehicle
- In-Car Commerce
- Location
- Navigation
- Marketing
- Germany
---
