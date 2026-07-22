---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: lumere.com
  spf: true
hosts:
- cert_expires: Feb 18 23:59:59 2027 GMT
  host: lumere.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Lumere Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Lumere, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Lumere
provider_slug: lumere
slug: lumere-domain-security
source_filename: lumere-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: lumere.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Feb 18 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: lumere.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lumere/refs/heads/main/security/lumere-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Company
- Healthcare
- Medical Devices
- Clinical Analytics
- Supply Chain
- Value Analysis
- Acquired
---
