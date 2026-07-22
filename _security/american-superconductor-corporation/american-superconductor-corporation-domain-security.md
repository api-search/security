---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: amsc.com
  spf: true
hosts:
- cert_expires: Aug 19 14:09:39 2026 GMT
  host: www.amsc.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: American Superconductor Corporation Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for American Superconductor Corporation, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: American Superconductor Corporation
provider_slug: american-superconductor-corporation
slug: american-superconductor-corporation-domain-security
source_filename: american-superconductor-corporation-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.amsc.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 19 14:09:39 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: amsc.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/american-superconductor-corporation/refs/heads/main/security/american-superconductor-corporation-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Hardtech
- Energy
- Renewables
- Power Grid
- Superconductors
- Industrials
- Utility
- Military
- Defense
---
