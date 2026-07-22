---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: homelane.com
  spf: true
hosts:
- cert_expires: Sep 12 06:10:46 2026 GMT
  host: www.homelane.com
  hsts: true
  hsts_max_age: 0
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Homelane Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for HomeLane, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: HomeLane
provider_slug: homelane
slug: homelane-domain-security
source_filename: homelane-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.homelane.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 12 06:10:46 2026 GMT\n  hsts: true\n  hsts_max_age: 0\ndomains:\n- domain: homelane.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/homelane/refs/heads/main/security/homelane-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Consumer
- Interior Design
- Home Services
- Home Improvement
- Furniture
- Modular Kitchen
- Retail
- India
---
