---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: hubs.com
  spf: true
hosts:
- cert_expires: Jan  4 23:59:59 2027 GMT
  host: www.hubs.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Hubs Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for hubs, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: hubs
provider_slug: hubs
slug: hubs-domain-security
source_filename: hubs-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.hubs.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  4 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: hubs.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hubs/refs/heads/main/security/hubs-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Manufacturing
- On-Demand Manufacturing
- Digital Manufacturing
- 3D Printing
- CNC Machining
- Injection Molding
- Sheet Metal Fabrication
- Hardware
---
