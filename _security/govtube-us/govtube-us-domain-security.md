---
api_specs:
- filename: govtube-us-citations-api-openapi.yml
  format: yaml
  label: GovTube Citations API
  slug: govtube-us-citations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/govtube-us/openapi/govtube-us-citations-api-openapi.yml
- filename: govtube-us-coverage-api-openapi.yml
  format: yaml
  label: GovTube Coverage API
  slug: govtube-us-coverage-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/govtube-us/openapi/govtube-us-coverage-api-openapi.yml
- filename: govtube-us-healthz-api-openapi.yml
  format: yaml
  label: GovTube Healthz API
  slug: govtube-us-healthz-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/govtube-us/openapi/govtube-us-healthz-api-openapi.yml
- filename: govtube-us-search-api-openapi.yml
  format: yaml
  label: GovTube Search API
  slug: govtube-us-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/govtube-us/openapi/govtube-us-search-api-openapi.yml
- filename: govtube-us-speakers-api-openapi.yml
  format: yaml
  label: GovTube Speakers API
  slug: govtube-us-speakers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/govtube-us/openapi/govtube-us-speakers-api-openapi.yml
- filename: govtube-us-videos-api-openapi.yml
  format: yaml
  label: GovTube Videos API
  slug: govtube-us-videos-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/govtube-us/openapi/govtube-us-videos-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: govtube.us
  spf: true
hosts:
- cert_expires: Jan 10 00:49:52 2027 GMT
  host: govtube.us
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: GovTube Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for GovTube, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: GovTube
provider_slug: govtube-us
slug: govtube-us-domain-security
source_filename: govtube-us-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-10'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: govtube.us\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 10 00:49:52 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: govtube.us\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/govtube-us/security/govtube-us-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Search
- Government
- Video
- Free
---
