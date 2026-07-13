---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: acnhapi.com
  spf: true
hosts:
- cert_expires: Aug 10 22:03:28 2026 GMT
  host: acnhapi.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Animal Crossing New Horizons Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Animal Crossing: New Horizons, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: 'Animal Crossing: New Horizons'
provider_slug: animal-crossing-new-horizons
slug: animal-crossing-new-horizons-domain-security
source_filename: animal-crossing-new-horizons-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: acnhapi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 10 22:03:28 2026 GMT\n  hsts: null\ndomains:\n- domain: acnhapi.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/animal-crossing-new-horizons/refs/heads/main/security/animal-crossing-new-horizons-domain-security.yml
summary_line: TLSv1.3
tags:
- Games And Comics
- Public APIs
---
