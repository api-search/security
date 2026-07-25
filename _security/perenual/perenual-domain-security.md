---
api_specs:
- filename: perenual-care-api-openapi.yml
  format: yaml
  label: Perenual Care API
  slug: perenual-care-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/perenual/refs/heads/main/openapi/perenual-care-api-openapi.yml
- filename: perenual-maps-api-openapi.yml
  format: yaml
  label: Perenual Maps API
  slug: perenual-maps-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/perenual/refs/heads/main/openapi/perenual-maps-api-openapi.yml
- filename: perenual-pests-api-openapi.yml
  format: yaml
  label: Perenual Pests API
  slug: perenual-pests-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/perenual/refs/heads/main/openapi/perenual-pests-api-openapi.yml
- filename: perenual-species-api-openapi.yml
  format: yaml
  label: Perenual Species API
  slug: perenual-species-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/perenual/refs/heads/main/openapi/perenual-species-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: perenual.com
  spf: true
hosts:
- cert_expires: Sep 26 11:32:07 2026 GMT
  host: perenual.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Perenual Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Perenual, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Perenual
provider_slug: perenual
slug: perenual-domain-security
source_filename: perenual-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: perenual.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 11:32:07 2026 GMT\n  hsts: false\ndomains:\n- domain: perenual.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/perenual/refs/heads/main/security/perenual-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Plants
- Botany
- Gardening
- Horticulture
---
