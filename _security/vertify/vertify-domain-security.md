---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: vertify.com
  spf: true
hosts:
- cert_expires: Nov 28 15:31:47 2026 GMT
  host: vertify.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Vertify Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Vertify, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Vertify
provider_slug: vertify
slug: vertify-domain-security
source_filename: vertify-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: vertify.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 28 15:31:47 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: vertify.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/vertify/security/vertify-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Revenue Operations
- Automation
- Data Integration
- Software-as-a-Service
---
