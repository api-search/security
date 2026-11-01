---
api_specs:
- filename: fastn-fastn-api-api-openapi.yml
  format: yaml
  label: Fastn API
  slug: fastn-api-2
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fastn/openapi/fastn-fastn-api-api-openapi.yml
- filename: fastn-openapi-generated.yml
  format: yaml
  label: Fastn API
  slug: fastn-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fastn/openapi/_ae-authored/fastn-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: fastn.ai
  spf: true
hosts:
- cert_expires: Dec 17 05:28:30 2026 GMT
  host: fastn.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Fastn Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Fastn, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Fastn
provider_slug: fastn
slug: fastn-domain-security
source_filename: fastn-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: fastn.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 17 05:28:30 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: fastn.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/fastn/security/fastn-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Integration Platform
- B2B SaaS
- Embedded Widget
- Unified API
- Data Integration
- AI Agents
- CRM Integration
- Security
---
