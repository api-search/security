---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: gevernova.com
  spf: true
hosts:
- cert_expires: Aug 19 20:14:40 2026 GMT
  host: www.gevernova.com
  hsts: true
  hsts_max_age: 86400
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ge Vernova Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for GE Vernova, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: GE Vernova
provider_slug: ge-vernova
slug: ge-vernova-domain-security
source_filename: ge-vernova-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.gevernova.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 19 20:14:40 2026 GMT\n  hsts: true\n  hsts_max_age: 86400\ndomains:\n- domain: gevernova.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ge-vernova/refs/heads/main/security/ge-vernova-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Decarbonization
- Electrification
- Energy
- Fortune 500
- Power
- Renewable Energy
- Sustainability
---
