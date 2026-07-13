---
api_specs:
- filename: revolutio-hazard-api-openapi.yml
  format: yaml
  label: Revolutio Hazard API
  slug: revolutio-hazard-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/revolutio/refs/heads/main/openapi/revolutio-hazard-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: revolutio.com.au
  spf: true
hosts:
- cert_expires: Aug 24 15:32:55 2026 GMT
  host: www.revolutio.com.au
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 25 23:59:59 2026 GMT
  host: api.revolutio.com.au
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Revolutio Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Revolutio, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Revolutio
provider_slug: revolutio
slug: revolutio-domain-security
source_filename: revolutio-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.revolutio.com.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 15:32:55 2026 GMT\n  hsts: false\n- host: api.revolutio.com.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 25 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: revolutio.com.au\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/revolutio/refs/heads/main/security/revolutio-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Engineering
- Hazard
- Weather
- Structural Engineering
- Wind Analysis
- Construction
---
