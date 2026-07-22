---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: whill.inc
  spf: true
hosts:
- cert_expires: Mar  9 23:59:59 2027 GMT
  host: whill.inc
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Whill Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Whill, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Whill
provider_slug: whill
slug: whill-domain-security
source_filename: whill-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: whill.inc\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar  9 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: whill.inc\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/whill/refs/heads/main/security/whill-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Mobility
- Personal Mobility
- Wheelchairs
- Mobility Scooters
- Autonomous Vehicles
- Hardware
- Healthcare
---
