---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: superplastic.co
  spf: false
hosts:
- cert_expires: Sep  8 01:18:02 2026 GMT
  host: superplastic.co
  hsts: true
  hsts_max_age: 7889238
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Superplastic Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Superplastic, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: Superplastic
provider_slug: superplastic
slug: superplastic-domain-security
source_filename: superplastic-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: superplastic.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  8 01:18:02 2026 GMT\n  hsts: true\n  hsts_max_age: 7889238\ndomains:\n- domain: superplastic.co\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/superplastic/refs/heads/main/security/superplastic-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Designer Toys
- Collectibles
- Entertainment
- E-Commerce
- Animation
- Consumer Brand
---
