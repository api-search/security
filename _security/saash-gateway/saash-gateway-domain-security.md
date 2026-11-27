---
api_specs:
- filename: saash-gateway-connector-api-openapi.yml
  format: yaml
  label: SAASH Connector API
  slug: saash-gateway-connector-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/saash-gateway/openapi/saash-gateway-connector-api-openapi.yml
- filename: saash-gateway-discovery-api-openapi.yml
  format: yaml
  label: SAASH Discovery API
  slug: saash-gateway-discovery-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/saash-gateway/openapi/saash-gateway-discovery-api-openapi.yml
- filename: saash-gateway-grow-api-openapi.yml
  format: yaml
  label: SAASH Grow API
  slug: saash-gateway-grow-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/saash-gateway/openapi/saash-gateway-grow-api-openapi.yml
- filename: saash-gateway-invoke-api-openapi.yml
  format: yaml
  label: SAASH Invoke API
  slug: saash-gateway-invoke-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/saash-gateway/openapi/saash-gateway-invoke-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: vercel.app
  spf: true
hosts:
- cert_expires: Nov 27 19:48:08 2026 GMT
  host: saash-gateway.vercel.app
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: SAASH Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SAASH, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: SAASH
provider_slug: saash-gateway
slug: saash-gateway-domain-security
source_filename: saash-gateway-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: saash-gateway.vercel.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 27 19:48:08 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: vercel.app\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/saash-gateway/security/saash-gateway-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
---
