---
api_specs:
- filename: dazie-io-account-api-openapi.yml
  format: yaml
  label: dazie Account API
  slug: dazie-io-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dazie-io/openapi/dazie-io-account-api-openapi.yml
- filename: dazie-io-calls-api-openapi.yml
  format: yaml
  label: dazie Calls API
  slug: dazie-io-calls-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dazie-io/openapi/dazie-io-calls-api-openapi.yml
- filename: dazie-io-journal-api-openapi.yml
  format: yaml
  label: dazie Journal API
  slug: dazie-io-journal-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dazie-io/openapi/dazie-io-journal-api-openapi.yml
- filename: dazie-io-memories-api-openapi.yml
  format: yaml
  label: dazie Memories API
  slug: dazie-io-memories-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dazie-io/openapi/dazie-io-memories-api-openapi.yml
- filename: dazie-io-to-dos-api-openapi.yml
  format: yaml
  label: dazie To Dos API
  slug: dazie-io-to-dos-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dazie-io/openapi/dazie-io-to-dos-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: dazie.io
  spf: true
hosts:
- cert_expires: Jan 18 02:03:14 2027 GMT
  host: dazie.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: dazie Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for dazie, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: dazie
provider_slug: dazie-io
slug: dazie-io-domain-security
source_filename: dazie-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: dazie.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 18 02:03:14 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: dazie.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/dazie-io/security/dazie-io-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Voice
- Journaling
- Artificial Intelligence
- Productivity
- Early-Access
---
