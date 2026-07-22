---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: owner.com
  spf: true
hosts:
- cert_expires: Sep 30 21:27:38 2026 GMT
  host: www.owner.com
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Owner Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Owner.com, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Owner.com
provider_slug: owner-com
slug: owner-com-domain-security
source_filename: owner-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.owner.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 21:27:38 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\ndomains:\n- domain: owner.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/owner-com/refs/heads/main/security/owner-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Restaurants
- Online Ordering
- Restaurant Marketing
- Loyalty
- Website Builder
- Food and Beverage
- SMB
- SaaS
- No Public API
---
