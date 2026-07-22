---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: nimanow.com
  spf: true
hosts:
- cert_expires: Oct 15 00:39:02 2026 GMT
  host: nimanow.com
  hsts: true
  hsts_max_age: 7889238
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Nimasensor Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for NimaSensor, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: NimaSensor
provider_slug: nimasensor
slug: nimasensor-domain-security
source_filename: nimasensor-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: nimanow.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 15 00:39:02 2026 GMT\n  hsts: true\n  hsts_max_age: 7889238\ndomains:\n- domain: nimanow.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nimasensor/refs/heads/main/security/nimasensor-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Health
- Consumer Hardware
- Food Safety
- Gluten
- Celiac
- E-Commerce
- IoT
---
