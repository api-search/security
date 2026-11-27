---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: safee.com
  spf: true
hosts:
- cert_expires: Dec 21 06:26:54 2026 GMT
  host: safee.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Safee Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Safee, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Safee
provider_slug: safee
slug: safee-domain-security
source_filename: safee-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-15'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: safee.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 21 06:26:54 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: safee.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/safee/security/safee-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Fleet Management
- Telematics
- GPS Tracking
- Vehicle-Analytics
- Software-as-a-Service
---
