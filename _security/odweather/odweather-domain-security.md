---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: oceandrivers.com
  spf: true
hosts:
- cert_expires: Sep 29 11:43:23 2026 GMT
  host: api.oceandrivers.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Odweather Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ODWeather, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: ODWeather
provider_slug: odweather
slug: odweather-domain-security
source_filename: odweather-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: api.oceandrivers.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 11:43:23 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: oceandrivers.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/odweather/refs/heads/main/security/odweather-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Weather
- Public APIs
---
