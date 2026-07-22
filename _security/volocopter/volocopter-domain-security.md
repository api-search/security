---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: volocopter.com
  spf: true
hosts:
- cert_expires: Aug 15 13:00:01 2026 GMT
  host: www.volocopter.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Volocopter Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Volocopter, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Volocopter
provider_slug: volocopter
slug: volocopter-domain-security
source_filename: volocopter-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.volocopter.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 15 13:00:01 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: volocopter.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/volocopter/refs/heads/main/security/volocopter-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Advanced Air Mobility
- Aerospace
- Air Taxi
- Cargo Drones
- EASA Certification
- eVTOL
- Electric Aviation
- Germany
- Multicopter
- Urban Air Mobility
---
