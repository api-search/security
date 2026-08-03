---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: 24-m.com
  spf: true
hosts:
- cert_expires: Oct 25 23:52:20 2026 GMT
  host: 24-m.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: 24M Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for 24M, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: 24M
provider_slug: 24m
slug: 24m-domain-security
source_filename: 24m-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: 24-m.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 25 23:52:20 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: 24-m.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/24m/refs/heads/main/security/24m-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Batteries
- Energy Storage
- Electric Vehicles
- Lithium-Ion
- Materials Science
- Manufacturing
- Clean Technology
- Hardware
---
