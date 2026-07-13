---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: pirateweather.net
  spf: true
hosts:
- cert_expires: Feb 22 23:59:59 2027 GMT
  host: pirateweather.net
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Pirate Weather Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Pirate Weather, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Pirate Weather
provider_slug: pirate-weather
slug: pirate-weather-domain-security
source_filename: pirate-weather-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: pirateweather.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 22 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: pirateweather.net\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pirate-weather/refs/heads/main/security/pirate-weather-domain-security.yml
summary_line: TLSv1.3
tags:
- Weather
- Public APIs
---
