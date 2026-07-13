---
api_specs:
- filename: meteosource-air-quality-data-api-openapi.yml
  format: yaml
  label: MeteoSource Air Quality Data API
  slug: meteosource-air-quality-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/meteosource-air-quality-data-api/refs/heads/main/openapi/meteosource-air-quality-data-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: meteosource.com
  spf: true
hosts:
- cert_expires: Sep  8 11:25:29 2026 GMT
  host: www.meteosource.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Meteosource Air Quality Data Api Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for MeteoSource Air Quality Data API, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: MeteoSource Air Quality Data API
provider_slug: meteosource-air-quality-data-api
slug: meteosource-air-quality-data-api-domain-security
source_filename: meteosource-air-quality-data-api-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.meteosource.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  8 11:25:29 2026 GMT\n  hsts: false\ndomains:\n- domain: meteosource.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/meteosource-air-quality-data-api/refs/heads/main/security/meteosource-air-quality-data-api-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Air Quality
- Environmental Data
- Forecasting
- Weather
---
