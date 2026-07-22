---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: byd.com
  spf: true
hosts:
- cert_expires: Mar  6 01:56:06 2027 GMT
  host: byd.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Byd Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for BYD, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: BYD
provider_slug: byd
slug: byd-domain-security
source_filename: byd-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: byd.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar  6 01:56:06 2027 GMT\n  hsts: false\ndomains:\n- domain: byd.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/byd/refs/heads/main/security/byd-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Technology
- Electric Vehicles
- Automotive
- Batteries
- Energy Storage
- Electronics
- Manufacturing
- Rail Transit
---
