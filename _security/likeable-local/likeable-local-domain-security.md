---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: storytellit.com
  spf: false
hosts:
- cert_expires: Sep 13 06:08:51 2026 GMT
  host: storytellit.com
  hsts: true
  hsts_max_age: 15768000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Likeable Local Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Likeable Local, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Likeable Local
provider_slug: likeable-local
slug: likeable-local-domain-security
source_filename: likeable-local-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: storytellit.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 06:08:51 2026 GMT\n  hsts: true\n  hsts_max_age: 15768000\ndomains:\n- domain: storytellit.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/likeable-local/refs/heads/main/security/likeable-local-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Social Media
- Marketing
- Social Media Management
- Advertising
- Small Business
- Agencies
- SaaS
---
