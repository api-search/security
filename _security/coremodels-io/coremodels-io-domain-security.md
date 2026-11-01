---
api_specs:
- filename: coremodels-io-integrationapi-api-openapi.yml
  format: yaml
  label: coremodels-io Integration API
  slug: coremodels-io-integrationapi-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coremodels-io/openapi/coremodels-io-integrationapi-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: coremodels.io
  spf: true
hosts:
- cert_expires: Jan 26 22:27:17 2027 GMT
  host: coremodels.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Coremodels Io Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for coremodels-io, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: coremodels-io
provider_slug: coremodels-io
slug: coremodels-io-domain-security
source_filename: coremodels-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: coremodels.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 26 22:27:17 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: coremodels.io\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/coremodels-io/security/coremodels-io-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Data-Modeling
- API-Platform
- Integration
- Schema-Mapping
---
