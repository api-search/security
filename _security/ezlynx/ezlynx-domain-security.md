---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: ezlynx.com
  spf: true
hosts:
- cert_expires: Sep 23 09:14:16 2026 GMT
  host: www.ezlynx.com
  hsts: true
  hsts_max_age: 15768000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ezlynx Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for EZLynx, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: EZLynx
provider_slug: ezlynx
slug: ezlynx-domain-security
source_filename: ezlynx-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.ezlynx.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 09:14:16 2026 GMT\n  hsts: true\n  hsts_max_age: 15768000\ndomains:\n- domain: ezlynx.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ezlynx/refs/heads/main/security/ezlynx-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Insurance
- InsurTech
- Comparative Rating
- Agency Management System
- CRM
- Quoting
- Property and Casualty
- Applied Systems
---
