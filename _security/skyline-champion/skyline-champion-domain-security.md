---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: skylinechampion.com
  spf: false
hosts:
- cert_expires: Nov 29 23:59:59 2026 GMT
  host: www.skylinechampion.com
  hsts: false
  https: true
  tls_version: TLSv1.2
- host: developer.skylinechampion.com
  https: false
- host: api.skylinechampion.com
  https: false
kind: domain-security
layout: security
method: probed
name: Skyline Champion Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Skyline Champion, probed live across 3 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: Skyline Champion
provider_slug: skyline-champion
slug: skyline-champion-domain-security
source_filename: skyline-champion-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.skylinechampion.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov 29 23:59:59 2026 GMT\n  hsts: false\n- host: developer.skylinechampion.com\n  https: false\n- host: api.skylinechampion.com\n  https: false\ndomains:\n- domain: skylinechampion.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/skyline-champion/refs/heads/main/security/skyline-champion-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- Manufactured Homes
- Housing
---
