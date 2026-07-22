---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: unitedmasters.com
  spf: true
hosts:
- cert_expires: Oct  1 23:59:59 2026 GMT
  host: unitedmasters.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Unitedmasters Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for UnitedMasters, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: UnitedMasters
provider_slug: unitedmasters
slug: unitedmasters-domain-security
source_filename: unitedmasters-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: unitedmasters.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: unitedmasters.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/unitedmasters/refs/heads/main/security/unitedmasters-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Music
- Music Distribution
- Streaming
- Royalties
- Creator Economy
- Entertainment
- Media
---
