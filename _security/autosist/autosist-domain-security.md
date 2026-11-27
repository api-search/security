---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: autosist.com
  spf: true
hosts:
- cert_expires: May  1 23:59:59 2027 GMT
  host: autosist.com
  hsts: false
  https: true
  tls_version: TLSv1.2
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: AUTOsist Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AUTOsist, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: AUTOsist
provider_slug: autosist
slug: autosist-domain-security
source_filename: autosist-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-15'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: autosist.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: May  1 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: autosist.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/autosist/security/autosist-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- Fleet Management
- Maintenance
- Software
- Software-as-a-Service
- Vehicles
---
