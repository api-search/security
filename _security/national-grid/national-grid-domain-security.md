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
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: neso.energy
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: carbonintensity.org.uk
  spf: false
hosts:
- cert_expires: Aug 30 15:27:23 2026 GMT
  host: www.neso.energy
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
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
name: National Grid Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for National Grid ESO, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: National Grid ESO
provider_slug: national-grid
slug: national-grid-domain-security
source_filename: national-grid-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.neso.energy\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 30 15:27:23 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: carbonintensity.org.uk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  3 23:59:59 2026 GMT\n  hsts: false\n- host: api.carbonintensity.org.uk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: neso.energy\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: carbonintensity.org.uk\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/national-grid/refs/heads/main/security/national-grid-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Energy
- Electricity
- Carbon Intensity
- UK
- Open Data
- Sustainability
- Grid Operations
---
