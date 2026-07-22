---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: mill.com
  spf: true
hosts:
- cert_expires: Sep 30 08:07:40 2026 GMT
  host: www.mill.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Mill Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Mill, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Mill
provider_slug: mill
slug: mill-domain-security
source_filename: mill-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.mill.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 08:07:40 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: mill.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mill/refs/heads/main/security/mill-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Consumer
- Food Waste
- Sustainability
- Composting
- Smart Home
- Hardware
- Climate
---
