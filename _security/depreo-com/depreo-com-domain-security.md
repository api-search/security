---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: depreo.com
  spf: true
hosts:
- cert_expires: Feb  1 02:44:08 2027 GMT
  host: depreo.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Depreo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Depreo, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Depreo
provider_slug: depreo-com
slug: depreo-com-domain-security
source_filename: depreo-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: depreo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  1 02:44:08 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: depreo.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/depreo-com/security/depreo-com-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Asset Management
- Depreciation
- IT Inventory
- Small Business
---
