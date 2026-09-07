---
api_specs:
- filename: openapi.json
  format: json
  label: RoxyAPI REST API v2
  slug: roxyapi-rest-api-v2
  spec_type: OpenAPI
  url: https://roxyapi.com/api/v2/openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: roxyapi.com
  spf: true
hosts:
- cert_expires: Oct 24 19:53:58 2026 GMT
  host: roxyapi.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Roxyapi Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for RoxyAPI, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: RoxyAPI
provider_slug: roxyapi
slug: roxyapi-domain-security
source_filename: roxyapi-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-03'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: roxyapi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 24 19:53:58 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: roxyapi.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/roxyapi/refs/heads/main/security/roxyapi-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Astrology
- Vedic Astrology
- numerology
- tarot
- human-design
- Forecast
- biorhythm
- iching
- crystals
- Dreams
- angel-numbers
- Location
- spiritual
- Wellness
- MCP Server
- OpenAPI
- llms-txt
- agent-native
---
