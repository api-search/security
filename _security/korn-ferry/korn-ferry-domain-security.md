---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: kornferry.com
  spf: true
hosts:
- cert_expires: Sep 16 22:31:21 2026 GMT
  host: www.kornferry.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Korn Ferry Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Korn Ferry, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Korn Ferry
provider_slug: korn-ferry
slug: korn-ferry-domain-security
source_filename: korn-ferry-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.kornferry.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 22:31:21 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: kornferry.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/korn-ferry/refs/heads/main/security/korn-ferry-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Consulting
- Talent Management
- Executive Search
- Human Resources
- Leadership Development
---
