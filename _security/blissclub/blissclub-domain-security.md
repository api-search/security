---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: blissclub.com
  spf: true
hosts:
- cert_expires: Nov  5 03:09:32 2026 GMT
  host: blissclub.com
  hsts: true
  hsts_max_age: 7889238
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Blissclub Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Blissclub, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Blissclub
provider_slug: blissclub
slug: blissclub-domain-security
source_filename: blissclub-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: blissclub.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  5 03:09:32 2026 GMT\n  hsts: true\n  hsts_max_age: 7889238\ndomains:\n- domain: blissclub.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/blissclub/refs/heads/main/security/blissclub-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Apparel
- E-Commerce
- Fashion
- Activewear
- Indian
---
