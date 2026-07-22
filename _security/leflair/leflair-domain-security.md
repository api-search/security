---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: leflair.com
  spf: false
hosts:
- cert_expires: Aug  4 09:04:31 2026 GMT
  host: leflair.com
  hsts: true
  hsts_max_age: 604800
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Leflair Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Leflair, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Leflair
provider_slug: leflair
slug: leflair-domain-security
source_filename: leflair-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: leflair.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug  4 09:04:31 2026 GMT\n  hsts: true\n  hsts_max_age: 604800\ndomains:\n- domain: leflair.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/leflair/refs/heads/main/security/leflair-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- E-Commerce
- Retail
- Vietnam
- Fashion
- Beauty
- Flash Sales
- Consumer
---
