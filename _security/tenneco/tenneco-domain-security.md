---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: tenneco.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: driv.com
  spf: true
hosts:
- cert_expires: Jan  6 23:59:59 2027 GMT
  host: www.tenneco.com
  hsts: true
  hsts_max_age: 31557600
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 15 03:44:05 2026 GMT
  host: www.driv.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Tenneco Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Tenneco, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Tenneco
provider_slug: tenneco
slug: tenneco-domain-security
source_filename: tenneco-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.tenneco.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  6 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31557600\n- host: www.driv.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 15 03:44:05 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: tenneco.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: driv.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tenneco/refs/heads/main/security/tenneco-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Aftermarket
- Automotive
- Emissions Control
- Manufacturing
- Powertrain
- Ride Performance
- Fortune 500
---
