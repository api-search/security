---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: sennder.com
  spf: true
hosts:
- cert_expires: Oct  5 21:03:44 2026 GMT
  host: www.sennder.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Sennder Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for sennder, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: sennder
provider_slug: sennder
slug: sennder-domain-security
source_filename: sennder-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.sennder.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 21:03:44 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: sennder.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sennder/refs/heads/main/security/sennder-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Carriers
- Digital Freight
- Europe
- Freight Forwarding
- Logistics
- Road Freight
- Shippers
- Supply Chain
- TMS Integration
- Transportation
---
