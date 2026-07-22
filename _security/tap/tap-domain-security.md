---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: tap3d.com
  spf: true
hosts:
- cert_expires: Sep 28 01:46:55 2026 GMT
  host: tap3d.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Tap Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Tap, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC absent.'
provider_name: Tap
provider_slug: tap
slug: tap-domain-security
source_filename: tap-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: tap3d.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 01:46:55 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: tap3d.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tap/refs/heads/main/security/tap-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC
tags:
- Company
- Training
- Manufacturing
- Virtual Reality
- Workforce Development
- Education
- Skills Assessment
- eLearning
---
