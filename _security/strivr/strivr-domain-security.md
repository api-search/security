---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: strivr.com
  spf: true
hosts:
- cert_expires: Oct  3 13:09:46 2026 GMT
  host: www.strivr.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  3 17:16:32 2026 GMT
  host: developer.strivr.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 26 15:25:43 2026 GMT
  host: api.strivr.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Strivr Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Strivr, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Strivr
provider_slug: strivr
slug: strivr-domain-security
source_filename: strivr-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.strivr.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 13:09:46 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.strivr.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  3 17:16:32 2026 GMT\n  hsts: false\n- host: api.strivr.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 26 15:25:43 2026 GMT\n  hsts: null\ndomains:\n- domain: strivr.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/strivr/refs/heads/main/security/strivr-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Immersive Learning
- Virtual Reality
- Workforce Training
- Frontline Operations
- Artificial Intelligence
- Analytics
- Unity SDK
- Smart Glasses
- Enterprise
- Learning and Development
---
