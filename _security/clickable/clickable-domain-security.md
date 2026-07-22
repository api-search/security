---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: clickable.com
  spf: true
hosts:
- cert_expires: Sep 18 07:14:42 2026 GMT
  host: clickable.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Clickable Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Clickable, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Clickable
provider_slug: clickable
slug: clickable-domain-security
source_filename: clickable-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: clickable.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 07:14:42 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: clickable.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/clickable/refs/heads/main/security/clickable-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Advertising
- Marketing
- Analytics
- PPC
- Reporting
- Automotive
- Search Advertising
- Social Advertising
---
