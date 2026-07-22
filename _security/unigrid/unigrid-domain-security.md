---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: unigridbattery.com
  spf: true
hosts:
- cert_expires: Aug 30 07:17:05 2026 GMT
  host: www.unigridbattery.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Unigrid Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Unigrid, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Unigrid
provider_slug: unigrid
slug: unigrid-domain-security
source_filename: unigrid-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.unigridbattery.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 30 07:17:05 2026 GMT\n  hsts: false\ndomains:\n- domain: unigridbattery.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/unigrid/refs/heads/main/security/unigrid-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Batteries
- Sodium-Ion
- Energy Storage
- Energy
- Hardware
- Data Centers
- Venture Backed
---
