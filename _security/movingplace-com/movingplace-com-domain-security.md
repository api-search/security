---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: movingplace.com
  spf: true
hosts:
- cert_expires: Dec 28 04:59:52 2026 GMT
  host: movingplace.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: MovingPlace Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for MovingPlace, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: MovingPlace
provider_slug: movingplace-com
slug: movingplace-com-domain-security
source_filename: movingplace-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: movingplace.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 28 04:59:52 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: movingplace.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/movingplace-com/security/movingplace-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Moving
- Marketplace
- Logistics
- Home Services
- United States
---
