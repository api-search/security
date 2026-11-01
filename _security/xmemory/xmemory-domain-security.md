---
api_specs:
- filename: xmemory-xmemory-api-api-openapi.yml
  format: yaml
  label: xmemory API
  slug: xmemory-api-2
  spec_type: OpenAPI
  url: https://artifacts.apis.io/xmemory/openapi/xmemory-xmemory-api-api-openapi.yml
- filename: xmemory-openapi-generated.yml
  format: yaml
  label: xmemory API
  slug: xmemory-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/xmemory/openapi/_ae-authored/xmemory-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: xmemory.ai
  spf: true
hosts:
- cert_expires: Dec 30 23:59:59 2026 GMT
  host: xmemory.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Xmemory Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for xmemory, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: xmemory
provider_slug: xmemory
slug: xmemory-domain-security
source_filename: xmemory-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: xmemory.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 30 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: xmemory.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/xmemory/security/xmemory-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Artificial Intelligence
- Memory
- Cloud
- Data Management
- Platform
---
