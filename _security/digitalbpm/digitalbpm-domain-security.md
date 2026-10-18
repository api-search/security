---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: digitalbpm.io
  spf: false
hosts:
- cert_expires: Jan 14 23:59:59 2027 GMT
  host: digitalbpm.io
  hsts: true
  hsts_max_age: 15768000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Digitalbpm Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for DigitalBPM, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: DigitalBPM
provider_slug: digitalbpm
slug: digitalbpm-domain-security
source_filename: digitalbpm-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: digitalbpm.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 14 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 15768000\ndomains:\n- domain: digitalbpm.io\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/digitalbpm/refs/heads/main/security/digitalbpm-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Automation
- No-Code
- Software-as-a-Service
- Integration
---
