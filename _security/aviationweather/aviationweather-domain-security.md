---
api_specs:
- filename: aviationweather-openapi.yml
  format: yaml
  label: Aviation Weather Data API
  slug: aviation-weather-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aviationweather/refs/heads/main/openapi/aviationweather-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: aviationweather.gov
  spf: false
hosts:
- cert_expires: Sep 19 23:59:59 2026 GMT
  host: aviationweather.gov
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Aviationweather Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Aviation Weather Center, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF absent, DMARC present (p=reject).'
provider_name: Aviation Weather Center
provider_slug: aviationweather
slug: aviationweather-domain-security
source_filename: aviationweather-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: aviationweather.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 19 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: aviationweather.gov\n  dnssec: true\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aviationweather/refs/heads/main/security/aviationweather-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Aviation
- Weather
- Government
- NOAA
- NWS
- METAR
- TAF
- PIREP
- SIGMET
- AIRMET
- Open Data
- Public APIs
---
