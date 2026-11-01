---
api_specs:
- filename: cosmic-ephemeris-calculations-api-openapi.yml
  format: yaml
  label: Cosmic Ephemeris Calculations API
  slug: cosmic-ephemeris-calculations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cosmic-ephemeris/openapi/cosmic-ephemeris-calculations-api-openapi.yml
- filename: cosmic-ephemeris-interpretation-api-openapi.yml
  format: yaml
  label: Cosmic Ephemeris Interpretation API
  slug: cosmic-ephemeris-interpretation-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cosmic-ephemeris/openapi/cosmic-ephemeris-interpretation-api-openapi.yml
- filename: cosmic-ephemeris-pro-timeline-api-openapi.yml
  format: yaml
  label: Cosmic Ephemeris Pro timeline API
  slug: cosmic-ephemeris-pro-timeline-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cosmic-ephemeris/openapi/cosmic-ephemeris-pro-timeline-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: cosmicephemeris.com
  spf: true
hosts:
- cert_expires: Jan  3 19:57:28 2027 GMT
  host: cosmicephemeris.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Cosmic Ephemeris Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cosmic Ephemeris, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Cosmic Ephemeris
provider_slug: cosmic-ephemeris
slug: cosmic-ephemeris-domain-security
source_filename: cosmic-ephemeris-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cosmicephemeris.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  3 19:57:28 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: cosmicephemeris.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/cosmic-ephemeris/security/cosmic-ephemeris-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Astrology
- API
- Developer
- Data
- U.S.-based
---
