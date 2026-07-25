---
api_specs:
- filename: horoscope-api-horoscope-api-openapi.yml
  format: yaml
  label: Horoscope API Horoscope API
  slug: horoscope-api-horoscope-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/horoscope-api/refs/heads/main/openapi/horoscope-api-horoscope-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: freehoroscopeapi.com
  spf: true
hosts:
- cert_expires: Sep 21 05:42:44 2026 GMT
  host: freehoroscopeapi.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Horoscope Api Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Horoscope API, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Horoscope API
provider_slug: horoscope-api
slug: horoscope-api-domain-security
source_filename: horoscope-api-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: freehoroscopeapi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 05:42:44 2026 GMT\n  hsts: false\ndomains:\n- domain: freehoroscopeapi.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/horoscope-api/refs/heads/main/security/horoscope-api-domain-security.yml
summary_line: TLSv1.3
tags:
- Astrology
- Content
- Horoscope
- Zodiac
---
