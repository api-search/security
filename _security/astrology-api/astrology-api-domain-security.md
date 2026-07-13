---
api_specs:
- filename: astrology-api-openapi.yml
  format: yaml
  label: Astrology API
  slug: astrology-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/astrology-api/refs/heads/main/openapi/astrology-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: astrologyapi.com
  spf: true
hosts:
- cert_expires: Sep 15 17:47:40 2026 GMT
  host: astrologyapi.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  3 23:59:59 2026 GMT
  host: json.astrologyapi.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Astrology Api Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Astrology API, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Astrology API
provider_slug: astrology-api
slug: astrology-api-domain-security
source_filename: astrology-api-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: astrologyapi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 17:47:40 2026 GMT\n  hsts: false\n- host: json.astrologyapi.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct  3 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: astrologyapi.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/astrology-api/refs/heads/main/security/astrology-api-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Astrology
- Horoscopes
- Zodiac
- Vedic Astrology
- Western Astrology
---
