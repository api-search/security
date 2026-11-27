---
api_specs:
- filename: thread-page-endpoint-urls-api-openapi.yml
  format: yaml
  label: ThreadPage Endpoint URLs API
  slug: thread-page-endpoint-urls-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/thread-page/openapi/thread-page-endpoint-urls-api-openapi.yml
- filename: thread-page-events-api-openapi.yml
  format: yaml
  label: ThreadPage Events API
  slug: thread-page-events-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/thread-page/openapi/thread-page-events-api-openapi.yml
- filename: thread-page-integration-api-api-openapi.yml
  format: yaml
  label: ThreadPage Integration API
  slug: thread-page-integration-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/thread-page/openapi/thread-page-integration-api-api-openapi.yml
- filename: thread-page-requests-api-openapi.yml
  format: yaml
  label: ThreadPage Requests API
  slug: thread-page-requests-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/thread-page/openapi/thread-page-requests-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: thread.page
  spf: true
hosts:
- cert_expires: Jan  4 21:56:12 2027 GMT
  host: thread.page
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: ThreadPage Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ThreadPage, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: ThreadPage
provider_slug: thread-page
slug: thread-page-domain-security
source_filename: thread-page-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-06'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: thread.page\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  4 21:56:12 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: thread.page\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/thread-page/security/thread-page-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Notes
- Collaboration
- Productivity
- Artificial Intelligence
- Web App
---
