---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: dayzim.com
  spf: true
hosts:
- cert_expires: Aug 28 01:46:52 2026 GMT
  host: www.dayzim.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Day Zimmermann Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Day & Zimmermann, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Day & Zimmermann
provider_slug: day-zimmermann
slug: day-zimmermann-domain-security
source_filename: day-zimmermann-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.dayzim.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 28 01:46:52 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: dayzim.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/day-zimmermann/refs/heads/main/security/day-zimmermann-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Ammunition
- Architecture and Engineering
- Construction
- Defense
- Engineering Services
- Government Services
- Industrial Services
- Maintenance
- Munitions
- Nuclear Services
- Power
- Staffing
- Workforce Solutions
---
