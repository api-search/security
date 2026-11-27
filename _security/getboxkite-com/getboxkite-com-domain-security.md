---
api_specs:
- filename: getboxkite-com-exports-api-openapi.yml
  format: yaml
  label: Boxkite Exports API
  slug: getboxkite-com-exports-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/getboxkite-com/openapi/getboxkite-com-exports-api-openapi.yml
- filename: getboxkite-com-organisations-api-openapi.yml
  format: yaml
  label: Boxkite Organisations API
  slug: getboxkite-com-organisations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/getboxkite-com/openapi/getboxkite-com-organisations-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: getboxkite.com
  spf: true
hosts:
- cert_expires: Feb  2 10:32:55 2027 GMT
  host: getboxkite.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Boxkite Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Boxkite, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Boxkite
provider_slug: getboxkite-com
slug: getboxkite-com-domain-security
source_filename: getboxkite-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-09'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: getboxkite.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  2 10:32:55 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: getboxkite.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/getboxkite-com/security/getboxkite-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Accounting
- Backup
- Cloud Storage
- New Zealand
- Small Business
---
