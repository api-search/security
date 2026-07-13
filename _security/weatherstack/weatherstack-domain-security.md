---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: weatherstack.com
  spf: true
hosts:
- cert_expires: Oct  8 18:04:12 2026 GMT
  host: weatherstack.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Weatherstack Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Weatherstack, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Weatherstack
provider_slug: weatherstack
slug: weatherstack-domain-security
source_filename: weatherstack-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: weatherstack.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 18:04:12 2026 GMT\n  hsts: false\ndomains:\n- domain: weatherstack.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/weatherstack/refs/heads/main/security/weatherstack-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Weather
- Public APIs
---
