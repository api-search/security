---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: anycreek.com
  spf: true
hosts:
- cert_expires: Dec 10 16:47:48 2026 GMT
  host: anycreek.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Anycreek Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AnyCreek, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: AnyCreek
provider_slug: anycreek
slug: anycreek-domain-security
source_filename: anycreek-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: anycreek.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 10 16:47:48 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: anycreek.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/anycreek/refs/heads/main/security/anycreek-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Payments
- Calendar Management
- Guide Assignments
- Marketing
- SEO
- Outdoor Guides
- Outfitters
---
