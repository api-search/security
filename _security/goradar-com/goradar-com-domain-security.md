---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: goradar.com
  spf: true
hosts:
- cert_expires: Jan 14 20:53:33 2027 GMT
  host: goradar.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Goradar Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Radar, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Radar
provider_slug: goradar-com
slug: goradar-com-domain-security
source_filename: goradar-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-24'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: goradar.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 14 20:53:33 2027 GMT\n  hsts: false\ndomains:\n- domain: goradar.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/goradar-com/security/goradar-com-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Retail
- RFID
- Inventory
- Automation
---
