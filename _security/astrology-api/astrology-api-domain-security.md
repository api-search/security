---
api_specs:
- filename: astrology-api-json-openapi.yml
  format: yaml
  label: Astrology API
  slug: astrology-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/astrology-api/refs/heads/main/openapi/astrology-api-json-openapi.yml
- filename: astrology-api-pdf-openapi.yml
  format: yaml
  label: AstrologyAPI PDF Reports API
  slug: astrology-api-pdf
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/astrology-api/refs/heads/main/openapi/astrology-api-pdf-openapi.yml
- filename: astrology-api-palmistry-openapi.json
  format: json
  label: AstrologyAPI Palmistry API
  slug: astrology-api-palmistry
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/astrology-api/refs/heads/main/openapi/astrology-api-palmistry-openapi.json
- filename: astrology-api-face-reading-openapi.yml
  format: yaml
  label: AstrologyAPI Face Reading API
  slug: astrology-api-face-reading
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/astrology-api/refs/heads/main/openapi/astrology-api-face-reading-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: astrologyapi.com
  spf: true
hosts:
- cert_expires: Nov 12 17:34:16 2026 GMT
  host: www.astrologyapi.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 13 21:33:19 2026 GMT
  host: astrologyapi.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar  5 23:59:59 2027 GMT
  host: json.astrologyapi.com
  hsts: null
  https: true
  tls_version: TLSv1.2
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Astrology Api Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Astrology API, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Astrology API
provider_slug: astrology-api
slug: astrology-api-domain-security
source_filename: astrology-api-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-07'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.astrologyapi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 12 17:34:16 2026 GMT\n  hsts: false\n- host: astrologyapi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 13 21:33:19 2026 GMT\n  hsts: false\n- host: json.astrologyapi.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Mar  5 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: astrologyapi.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/astrology-api/refs/heads/main/security/astrology-api-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Astrology
- Horoscopes
- Zodiac
- Vedic Astrology
- Western Astrology
- Kundli
- Panchang
- Numerology
- Tarot
- Palmistry
- Human Design
- Astrocartography
- PDF Reports
- MCP
- Ephemeris
---
