---
api_specs:
- filename: openaffiliate-dev-programs-api-openapi.yml
  format: yaml
  label: OpenAffiliate Programs API
  slug: openaffiliate-dev-programs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/openaffiliate-dev/openapi/openaffiliate-dev-programs-api-openapi.yml
- filename: openaffiliate-dev-submissions-api-openapi.yml
  format: yaml
  label: OpenAffiliate Submissions API
  slug: openaffiliate-dev-submissions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/openaffiliate-dev/openapi/openaffiliate-dev-submissions-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: openaffiliate.dev
  spf: true
hosts:
- cert_expires: Jan 17 15:44:04 2027 GMT
  host: openaffiliate.dev
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: OpenAffiliate Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for OpenAffiliate, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: OpenAffiliate
provider_slug: openaffiliate-dev
slug: openaffiliate-dev-domain-security
source_filename: openaffiliate-dev-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: openaffiliate.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 17 15:44:04 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: openaffiliate.dev\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/openaffiliate-dev/security/openaffiliate-dev-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Affiliates
- Marketing
- Directory
- Open Source
---
