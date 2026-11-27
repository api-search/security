---
api_specs:
- filename: openarchieven-nl-records-api-openapi.yml
  format: yaml
  label: Open Archives Records API
  slug: openarchieven-nl-records-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/openarchieven-nl/openapi/openarchieven-nl-records-api-openapi.yml
- filename: openarchieven-nl-related-api-openapi.yml
  format: yaml
  label: Open Archives Related API
  slug: openarchieven-nl-related-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/openarchieven-nl/openapi/openarchieven-nl-related-api-openapi.yml
- filename: openarchieven-nl-stats-api-openapi.yml
  format: yaml
  label: Open Archives Stats API
  slug: openarchieven-nl-stats-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/openarchieven-nl/openapi/openarchieven-nl-stats-api-openapi.yml
- filename: openarchieven-nl-transcriptions-api-openapi.yml
  format: yaml
  label: Open Archives Transcriptions API
  slug: openarchieven-nl-transcriptions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/openarchieven-nl/openapi/openarchieven-nl-transcriptions-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: openarchieven.nl
  spf: true
hosts:
- cert_expires: Jan 13 15:15:07 2027 GMT
  host: openarchieven.nl
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Open Archives Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Open Archives, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Open Archives
provider_slug: openarchieven-nl
slug: openarchieven-nl-domain-security
source_filename: openarchieven-nl-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: openarchieven.nl\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 13 15:15:07 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: openarchieven.nl\n  dnssec: true\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/openarchieven-nl/security/openarchieven-nl-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Genealogy
- Archives
- Dutch
- Open Data
- Search
---
