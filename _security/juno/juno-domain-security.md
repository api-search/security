---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: juno.co
  spf: false
hosts:
- cert_expires: Oct 16 07:35:09 2026 GMT
  host: juno.co
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Juno Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Juno, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: Juno
provider_slug: juno
slug: juno-domain-security
source_filename: juno-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-23'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: juno.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 16 07:35:09 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: juno.co\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/juno/refs/heads/main/security/juno-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Construction
- Construction Management
- Real-Estate
- Multifamily
- Prefabrication
- Modular Construction
- Mass Timber
- Property Technology
- Owner's Representation
- Sustainability
- Professional Services
---
