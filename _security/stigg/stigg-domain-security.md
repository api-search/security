---
api_specs:
- filename: stigg-openapi.yml
  format: yaml
  label: Stigg GraphQL API
  slug: stigg-graphql
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stigg/refs/heads/main/openapi/stigg-openapi.yml
- filename: stigg-rest-openapi.yml
  format: yaml
  label: Stigg REST API
  slug: stigg-rest
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stigg/refs/heads/main/openapi/stigg-rest-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: stigg.io
  spf: true
hosts:
- cert_expires: Sep 11 18:02:06 2026 GMT
  host: www.stigg.io
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  2 12:52:51 2026 GMT
  host: docs.stigg.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 25 23:59:59 2026 GMT
  host: api.stigg.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Stigg Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Stigg, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Stigg
provider_slug: stigg
slug: stigg-domain-security
source_filename: stigg-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.stigg.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 11 18:02:06 2026 GMT\n  hsts: false\n- host: docs.stigg.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 12:52:51 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.stigg.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 25 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: stigg.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/stigg/refs/heads/main/security/stigg-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- FinOps
- Pricing
- Billing
- Entitlements
- Usage-Based Billing
- Feature Flags
- Product-Led Growth
- Subscriptions
- SaaS
- GraphQL
- REST
---
