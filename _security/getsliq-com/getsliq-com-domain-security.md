---
api_specs:
- filename: getsliq-com-agents-api-openapi.yml
  format: yaml
  label: Sliq Agents API
  slug: getsliq-com-agents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/getsliq-com/openapi/getsliq-com-agents-api-openapi.yml
- filename: getsliq-com-people-api-openapi.yml
  format: yaml
  label: Sliq People API
  slug: getsliq-com-people-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/getsliq-com/openapi/getsliq-com-people-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: getsliq.com
  spf: true
hosts:
- cert_expires: Dec 26 21:48:11 2026 GMT
  host: getsliq.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Sliq Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Sliq, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Sliq
provider_slug: getsliq-com
slug: getsliq-com-domain-security
source_filename: getsliq-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-10'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: getsliq.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 26 21:48:11 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: getsliq.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/getsliq-com/security/getsliq-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Outbound Sales
- Sales Outreach
---
