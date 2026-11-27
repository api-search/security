---
api_specs:
- filename: namefi-io-admin-api-openapi.yml
  format: yaml
  label: Namefi Admin API
  slug: namefi-io-admin-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/namefi-io/openapi/namefi-io-admin-api-openapi.yml
- filename: namefi-io-auth-api-openapi.yml
  format: yaml
  label: Namefi Auth API
  slug: namefi-io-auth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/namefi-io/openapi/namefi-io-auth-api-openapi.yml
- filename: namefi-io-balance-api-openapi.yml
  format: yaml
  label: Namefi Balance API
  slug: namefi-io-balance-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/namefi-io/openapi/namefi-io-balance-api-openapi.yml
- filename: namefi-io-base-route-api-openapi.yml
  format: yaml
  label: Namefi Base Route API
  slug: namefi-io-base-route-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/namefi-io/openapi/namefi-io-base-route-api-openapi.yml
- filename: namefi-io-ddns-api-openapi.yml
  format: yaml
  label: Namefi Ddns API
  slug: namefi-io-ddns-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/namefi-io/openapi/namefi-io-ddns-api-openapi.yml
- filename: namefi-io-dns-api-openapi.yml
  format: yaml
  label: Namefi Dns API
  slug: namefi-io-dns-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/namefi-io/openapi/namefi-io-dns-api-openapi.yml
- filename: namefi-io-domain-config-api-openapi.yml
  format: yaml
  label: Namefi Domain Config API
  slug: namefi-io-domain-config-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/namefi-io/openapi/namefi-io-domain-config-api-openapi.yml
- filename: namefi-io-eip712-api-openapi.yml
  format: yaml
  label: Namefi Eip712 API
  slug: namefi-io-eip712-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/namefi-io/openapi/namefi-io-eip712-api-openapi.yml
- filename: namefi-io-oauth-api-openapi.yml
  format: yaml
  label: Namefi OAuth API
  slug: namefi-io-oauth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/namefi-io/openapi/namefi-io-oauth-api-openapi.yml
- filename: namefi-io-orders-api-openapi.yml
  format: yaml
  label: Namefi Orders API
  slug: namefi-io-orders-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/namefi-io/openapi/namefi-io-orders-api-openapi.yml
- filename: namefi-io-outbound-api-openapi.yml
  format: yaml
  label: Namefi Outbound API
  slug: namefi-io-outbound-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/namefi-io/openapi/namefi-io-outbound-api-openapi.yml
- filename: namefi-io-search-api-openapi.yml
  format: yaml
  label: Namefi Search API
  slug: namefi-io-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/namefi-io/openapi/namefi-io-search-api-openapi.yml
- filename: namefi-io-siwe-api-openapi.yml
  format: yaml
  label: Namefi Siwe API
  slug: namefi-io-siwe-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/namefi-io/openapi/namefi-io-siwe-api-openapi.yml
- filename: namefi-io-studio-api-openapi.yml
  format: yaml
  label: Namefi Studio API
  slug: namefi-io-studio-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/namefi-io/openapi/namefi-io-studio-api-openapi.yml
- filename: namefi-io-user-api-openapi.yml
  format: yaml
  label: Namefi User API
  slug: namefi-io-user-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/namefi-io/openapi/namefi-io-user-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: namefi.io
  spf: true
hosts:
- cert_expires: Jan  3 14:38:53 2027 GMT
  host: namefi.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Namefi Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Namefi, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Namefi
provider_slug: namefi-io
slug: namefi-io-domain-security
source_filename: namefi-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: namefi.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  3 14:38:53 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: namefi.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/namefi-io/security/namefi-io-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Domain Registrar
- Tokenized Domains
- AI Agents
- On‑chain Domains
---
