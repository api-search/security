---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: carbondesignsystem.com
  spf: false
hosts:
- cert_expires: Jan 17 12:24:20 2027 GMT
  host: carbondesignsystem.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Carbondesignsystem Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Carbon Design System, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF absent, DMARC present (p=none).'
provider_name: Carbon Design System
provider_slug: carbondesignsystem-com
slug: carbondesignsystem-com-domain-security
source_filename: carbondesignsystem-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: carbondesignsystem.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 17 12:24:20 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: carbondesignsystem.com\n  dnssec: true\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/carbondesignsystem-com/security/carbondesignsystem-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Design Systems
- Open Source
- UI Components
- Accessibility
- Digital Experience
- IBM
---
