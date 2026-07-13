---
api_specs:
- filename: stormglass-openapi.yml
  format: yaml
  label: Stormglass API
  slug: stormglass-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stormglass/refs/heads/main/openapi/stormglass-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: stormglass.io
  spf: true
hosts:
- cert_expires: Aug 25 10:06:21 2026 GMT
  host: stormglass.io
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 20 23:06:18 2026 GMT
  host: api.stormglass.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Stormglass Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Stormglass, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Stormglass
provider_slug: stormglass
slug: stormglass-domain-security
source_filename: stormglass-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: stormglass.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 25 10:06:21 2026 GMT\n  hsts: false\n- host: api.stormglass.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 23:06:18 2026 GMT\n  hsts: null\ndomains:\n- domain: stormglass.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/stormglass/refs/heads/main/security/stormglass-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Astronomy
- Bio
- Climate
- Elevation
- Forecasting
- Marine
- Ocean
- Solar
- Tides
- Weather
- Wind
---
