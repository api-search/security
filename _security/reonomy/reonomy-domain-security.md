---
api_specs:
- filename: reonomy-property-api-openapi.yml
  format: yaml
  label: Reonomy Property API
  slug: reonomy-property-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reonomy/refs/heads/main/openapi/reonomy-property-api-openapi.yml
- filename: reonomy-search-api-openapi.yml
  format: yaml
  label: Reonomy Search API
  slug: reonomy-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reonomy/refs/heads/main/openapi/reonomy-search-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: reonomy.com
  spf: true
hosts:
- cert_expires: Sep  1 17:18:54 2026 GMT
  host: www.reonomy.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  1 17:18:54 2026 GMT
  host: api.reonomy.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Reonomy Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Reonomy, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Reonomy
provider_slug: reonomy
slug: reonomy-domain-security
source_filename: reonomy-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.reonomy.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  1 17:18:54 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.reonomy.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  1 17:18:54 2026 GMT\n  hsts: null\ndomains:\n- domain: reonomy.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/reonomy/refs/heads/main/security/reonomy-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Commercial Real Estate
- Property Data
- Property Intelligence
- Ownership
- Skip Trace
---
