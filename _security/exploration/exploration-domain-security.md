---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: exploration.space
  spf: true
hosts:
- cert_expires: Sep 10 09:30:49 2026 GMT
  host: www.exploration.space
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Exploration Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for The Exploration Company, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: The Exploration Company
provider_slug: exploration
slug: exploration-domain-security
source_filename: exploration-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.exploration.space\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 10 09:30:49 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: exploration.space\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/exploration/refs/heads/main/security/exploration-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Space
- Aerospace
- Space Transportation
- Reusable Spacecraft
- Launch Vehicles
- Rocket Engines
- Deep Tech
- Hardware
---
