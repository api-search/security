---
api_specs:
- filename: rsc-filter-api-openapi.yml
  format: yaml
  label: RSC Filter API
  slug: rsc-filter-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rsc/refs/heads/main/openapi/rsc-filter-api-openapi.yml
- filename: rsc-lookups-api-openapi.yml
  format: yaml
  label: RSC Lookups API
  slug: rsc-lookups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rsc/refs/heads/main/openapi/rsc-lookups-api-openapi.yml
- filename: rsc-records-api-openapi.yml
  format: yaml
  label: RSC Records API
  slug: rsc-records-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rsc/refs/heads/main/openapi/rsc-records-api-openapi.yml
- filename: rsc-tools-api-openapi.yml
  format: yaml
  label: RSC Tools API
  slug: rsc-tools-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rsc/refs/heads/main/openapi/rsc-tools-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: rsc.org
  spf: true
hosts:
- cert_expires: Sep 25 23:59:59 2026 GMT
  host: developer.rsc.org
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 16 23:59:59 2026 GMT
  host: api.rsc.org
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Rsc Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for RSC, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: RSC
provider_slug: rsc
slug: rsc-domain-security
source_filename: rsc-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developer.rsc.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.rsc.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 16 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: rsc.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rsc/refs/heads/main/security/rsc-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Chemistry
- Cheminformatics
- Chemical Data
- Science
---
