---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: atmosfy.io
  spf: true
hosts:
- cert_expires: Dec 29 23:59:59 2026 GMT
  host: atmosfy.io
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Atmosfy Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Atmosfy, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Atmosfy
provider_slug: atmosfy
slug: atmosfy-domain-security
source_filename: atmosfy-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: atmosfy.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 29 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: atmosfy.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/atmosfy/refs/heads/main/security/atmosfy-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Video
- Maps
- Location
- Social
- Discovery
- Local
- Restaurants
- User Generated Content
- AI Training Data
---
