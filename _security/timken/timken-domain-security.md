---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: timken.com
  spf: true
hosts:
- cert_expires: Aug  8 05:35:00 2026 GMT
  host: www.timken.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug  8 05:36:40 2026 GMT
  host: engineering.timken.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Timken Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Timken, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Timken
provider_slug: timken
slug: timken-domain-security
source_filename: timken-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.timken.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug  8 05:35:00 2026 GMT\n  hsts: false\n- host: engineering.timken.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug  8 05:36:40 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: timken.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/timken/refs/heads/main/security/timken-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Bearings
- Industrial
- Manufacturing
- Motion Control
- Fortune 1000
---
