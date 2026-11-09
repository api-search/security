---
api_specs:
- filename: briq-cloud-v1-openapi.json
  format: json
  label: briq API V1 API
  slug: briq-api-v1-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/briq-cloud/openapi/_original/briq-cloud-v1-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: briq.cloud
  spf: true
hosts:
- cert_expires: Dec 25 09:17:02 2026 GMT
  host: briq.cloud
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Briq Cloud Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for briq, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: briq
provider_slug: briq-cloud
slug: briq-cloud-domain-security
source_filename: briq-cloud-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: briq.cloud\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 25 09:17:02 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: briq.cloud\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/briq-cloud/security/briq-cloud-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Artificial Intelligence
- Cloud
- Sandbox
- Database
- Platform
- Company
---
