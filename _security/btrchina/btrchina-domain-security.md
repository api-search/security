---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: btrchina.com
  spf: false
hosts:
- cert_expires: Dec 24 23:59:59 2026 GMT
  host: btrchina.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Btrchina Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for BTR New Material Group, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=quarantine).'
provider_name: BTR New Material Group
provider_slug: btrchina
slug: btrchina-domain-security
source_filename: btrchina-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: btrchina.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 24 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: btrchina.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/btrchina/refs/heads/main/security/btrchina-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Company
- Battery Materials
- Lithium-Ion Batteries
- Anode Materials
- Cathode Materials
- Advanced Materials
- Energy Storage
- Manufacturing
---
