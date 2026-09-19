---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: afalight.com
  spf: true
hosts:
- host: www.afalight.com
  hsts: true
  hsts_include_subdomains: false
  hsts_max_age: 31536000
  hsts_preload: false
  http_version: h2
  https: true
  observed: '2026-09-12'
  server: nginx
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Afalight Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Afalight, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS; 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Afalight
provider_slug: afalight
slug: afalight-domain-security
source_filename: afalight-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml hosts (no API baseURL or OpenAPI servers[] host exists)\nnote: >-\n  The automated probe (0-working/probe-domain-security.py) first recorded https: false for\n  www.afalight.com; that was a false negative caused by repeated connection timeouts against\n  this origin, which is slow and intermittent from a US vantage point. A direct HEAD confirmed\n  HTTP/2 200 over TLS with a Strict-Transport-Security header, so the corrected values below\n  are the observed ones.\nhosts:\n- host: www.afalight.com\n  https: true\n  http_version: h2\n  server: nginx\n  hsts: true\n  hsts_max_age: 31536000\n  hsts_include_subdomains: false\n  hsts_preload: false\n  observed: '2026-09-12'\ndomains:\n- domain: afalight.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/afalight/refs/heads/main/security/afalight-domain-security.yml
summary_line: HSTS · DMARC
tags:
- Company
- Hardware
- Optoelectronics
- Optical Modules
- Fiber Optics
- Video
- Manufacturing
- Semiconductors
- Consumer Electronics
- China
---
