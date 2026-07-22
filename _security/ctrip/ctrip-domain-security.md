---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: ctrip.com
  spf: true
hosts:
- cert_expires: Apr 12 09:11:55 2027 GMT
  host: ctrip.com
  hsts: true
  hsts_max_age: 120
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Ctrip Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ctrip, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Ctrip
provider_slug: ctrip
slug: ctrip-domain-security
source_filename: ctrip-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ctrip.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Apr 12 09:11:55 2027 GMT\n  hsts: true\n  hsts_max_age: 120\ndomains:\n- domain: ctrip.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ctrip/refs/heads/main/security/ctrip-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Company
- Consumer Technology
- Travel
- Online Travel Agency
- Hotels
- Flights
- Trip.com Group
- China
---
