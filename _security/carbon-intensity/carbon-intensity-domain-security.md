---
api_specs:
- filename: openapi.yaml
  format: yaml
  label: Carbon Intensity API
  slug: carbon-intensity-api
  spec_type: OpenAPI
  url: https://carbon-intensity.github.io/api-definitions/
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: carbonintensity.org.uk
  spf: false
hosts:
- cert_expires: Dec  3 23:59:59 2026 GMT
  host: carbonintensity.org.uk
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 21 23:59:59 2026 GMT
  host: api.carbonintensity.org.uk
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Carbon Intensity Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Carbon Intensity API, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Carbon Intensity API
provider_slug: carbon-intensity
slug: carbon-intensity-domain-security
source_filename: carbon-intensity-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: carbonintensity.org.uk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  3 23:59:59 2026 GMT\n  hsts: false\n- host: api.carbonintensity.org.uk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: carbonintensity.org.uk\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/carbon-intensity/refs/heads/main/security/carbon-intensity-domain-security.yml
summary_line: TLSv1.3
tags:
- Carbon Intensity
- Environment
- Energy
- Electricity
- Climate
- Great Britain
- National Grid
---
