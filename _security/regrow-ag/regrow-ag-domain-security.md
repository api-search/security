---
api_specs:
- filename: regrow-ag-ogc-api-general-api-openapi.yml
  format: yaml
  label: Regrow OGC API - General API
  slug: regrow-ag-ogc-api-general-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/regrow-ag/openapi/regrow-ag-ogc-api-general-api-openapi.yml
- filename: regrow-ag-ogc-api-processes-api-openapi.yml
  format: yaml
  label: Regrow OGC API - Processes API
  slug: regrow-ag-ogc-api-processes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/regrow-ag/openapi/regrow-ag-ogc-api-processes-api-openapi.yml
- filename: regrow-ag-v0-explore-api-intervention-api-openapi.yml
  format: yaml
  label: Regrow V0 Explore API - Intervention API
  slug: regrow-ag-v0-explore-api-intervention-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/regrow-ag/openapi/regrow-ag-v0-explore-api-intervention-api-openapi.yml
- filename: regrow-ag-v0-measure-api-intervention-api-openapi.yml
  format: yaml
  label: Regrow V0 Measure API - Intervention API
  slug: regrow-ag-v0-measure-api-intervention-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/regrow-ag/openapi/regrow-ag-v0-measure-api-intervention-api-openapi.yml
- filename: regrow-ag-v0-measure-api-inventory-api-openapi.yml
  format: yaml
  label: Regrow V0 Measure API - Inventory API
  slug: regrow-ag-v0-measure-api-inventory-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/regrow-ag/openapi/regrow-ag-v0-measure-api-inventory-api-openapi.yml
- filename: regrow-ag-v1-measure-api-enteric-api-openapi.yml
  format: yaml
  label: Regrow V1 Measure API - Enteric API
  slug: regrow-ag-v1-measure-api-enteric-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/regrow-ag/openapi/regrow-ag-v1-measure-api-enteric-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: regrow.ag
  spf: true
hosts:
- cert_expires: Jan 31 02:43:03 2027 GMT
  host: www.regrow.ag
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 22 03:24:10 2027 GMT
  host: developers.regrow.ag
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 22 22:23:06 2026 GMT
  host: api.regrow.ag
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Regrow Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Regrow, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Regrow
provider_slug: regrow-ag
slug: regrow-ag-domain-security
source_filename: regrow-ag-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-09'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.regrow.ag\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 31 02:43:03 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developers.regrow.ag\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 22 03:24:10 2027 GMT\n  hsts: null\n- host: api.regrow.ag\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 22 22:23:06 2026 GMT\n  hsts: null\ndomains:\n- domain: regrow.ag\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/regrow-ag/security/regrow-ag-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Agriculture
- Sustainability
- Greenhouse Gas Emissions
- Carbon
- Regenerative Agriculture
- Remote Sensing
- Climate
---
