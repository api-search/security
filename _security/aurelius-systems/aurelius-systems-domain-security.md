---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: aureliussystems.com
  spf: false
hosts:
- cert_expires: Aug 25 21:21:03 2026 GMT
  host: aureliussystems.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Aurelius Systems Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Aurelius Systems, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Aurelius Systems
provider_slug: aurelius-systems
slug: aurelius-systems-domain-security
source_filename: aurelius-systems-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: aureliussystems.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 25 21:21:03 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: aureliussystems.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aurelius-systems/refs/heads/main/security/aurelius-systems-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Defense Government
- Directed Energy
- Counter-UAS
- Drone Defense
- Autonomous Systems
- Laser
- National Security
---
