---
api_specs:
- filename: callforme-tel-account-api-openapi.yml
  format: yaml
  label: CallForMe Account API
  slug: callforme-tel-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/callforme-tel/openapi/callforme-tel-account-api-openapi.yml
- filename: callforme-tel-batches-api-openapi.yml
  format: yaml
  label: CallForMe Batches API
  slug: callforme-tel-batches-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/callforme-tel/openapi/callforme-tel-batches-api-openapi.yml
- filename: callforme-tel-businesses-api-openapi.yml
  format: yaml
  label: CallForMe Businesses API
  slug: callforme-tel-businesses-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/callforme-tel/openapi/callforme-tel-businesses-api-openapi.yml
- filename: callforme-tel-calls-api-openapi.yml
  format: yaml
  label: CallForMe Calls API
  slug: callforme-tel-calls-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/callforme-tel/openapi/callforme-tel-calls-api-openapi.yml
- filename: callforme-tel-pricing-api-openapi.yml
  format: yaml
  label: CallForMe Pricing API
  slug: callforme-tel-pricing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/callforme-tel/openapi/callforme-tel-pricing-api-openapi.yml
- filename: callforme-tel-setups-api-openapi.yml
  format: yaml
  label: CallForMe Setups API
  slug: callforme-tel-setups-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/callforme-tel/openapi/callforme-tel-setups-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: callforme.tel
  spf: true
hosts:
- cert_expires: Dec 28 06:03:23 2026 GMT
  host: callforme.tel
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: CallForMe Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CallForMe, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: CallForMe
provider_slug: callforme-tel
slug: callforme-tel-domain-security
source_filename: callforme-tel-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: callforme.tel\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 28 06:03:23 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: callforme.tel\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/callforme-tel/security/callforme-tel-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- AI Agents
- Voice
- Phone Calls
- Telephony
- MCP
- REST API
---
