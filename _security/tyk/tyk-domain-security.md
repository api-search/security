---
api_specs:
- filename: tyk-gateway-api-openapi.yml
  format: yaml
  label: Tyk Gateway API
  slug: tyk-gateway-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tyk/refs/heads/main/openapi/tyk-gateway-api-openapi.yml
- filename: tyk-dashboard-api-openapi.yml
  format: yaml
  label: Tyk Dashboard API
  slug: tyk-dashboard-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tyk/refs/heads/main/openapi/tyk-dashboard-api-openapi.yml
- filename: tyk-dashboard-admin-api-openapi.yml
  format: yaml
  label: Tyk Dashboard Admin API
  slug: tyk-dashboard-admin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tyk/refs/heads/main/openapi/tyk-dashboard-admin-api-openapi.yml
- filename: tyk-mdcb-api-openapi.yml
  format: yaml
  label: Tyk MDCB API
  slug: tyk-mdcb-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tyk/refs/heads/main/openapi/tyk-mdcb-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "ssl.com"
  - 0 issue "amazon.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: tyk.io
  spf: true
hosts:
- cert_expires: Sep  8 13:02:29 2026 GMT
  host: tyk.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Tyk Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Tyk, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Tyk
provider_slug: tyk
slug: tyk-domain-security
source_filename: tyk-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: tyk.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  8 13:02:29 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: tyk.io\n  dnssec: true\n  caa:\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tyk/refs/heads/main/security/tyk-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- API Gateway
- API Management
- GraphQL
- Open Source
---
