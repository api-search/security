---
api_specs:
- filename: moon-api-openapi.yml
  format: yaml
  label: Moon API
  slug: moon-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moon-api/refs/heads/main/openapi/moon-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: moon-api.com
  spf: true
- caa: []
  dmarc: false
  dnssec: true
  domain: rapidapi.com
  spf: true
hosts:
- cert_expires: Jan 14 23:59:59 2027 GMT
  host: moon-api.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 18 23:59:59 2026 GMT
  host: moon-phase.p.rapidapi.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Moon Api Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Moon-API, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Moon-API
provider_slug: moon-api
slug: moon-api-domain-security
source_filename: moon-api-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: moon-api.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 14 23:59:59 2027 GMT\n  hsts: false\n- host: moon-phase.p.rapidapi.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 18 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: moon-api.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: rapidapi.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/moon-api/refs/heads/main/security/moon-api-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Astrology
- Astronomy
- Lunar
- Moon
- Moon Phases
- Space
---
