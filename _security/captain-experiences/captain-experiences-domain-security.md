---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: captainexperiences.com
  spf: true
hosts:
- cert_expires: Dec 23 15:15:37 2026 GMT
  host: captainexperiences.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Captain Experiences Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Captain Experiences, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Captain Experiences
provider_slug: captain-experiences
slug: captain-experiences-domain-security
source_filename: captain-experiences-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-07'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: captainexperiences.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 23 15:15:37 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: captainexperiences.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/captain-experiences/refs/heads/main/security/captain-experiences-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Outdoors
- Travel
- Fishing
- Hunting
---
