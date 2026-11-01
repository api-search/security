---
api_specs:
- filename: scope-bid-carrier-feed-api-openapi.yml
  format: yaml
  label: scope-bid Carrier Feed API
  slug: scope-bid-carrier-feed-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/scope-bid/openapi/scope-bid-carrier-feed-api-openapi.yml
- filename: scope-bid-deliverables-api-openapi.yml
  format: yaml
  label: scope-bid Deliverables API
  slug: scope-bid-deliverables-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/scope-bid/openapi/scope-bid-deliverables-api-openapi.yml
- filename: scope-bid-dispatches-api-openapi.yml
  format: yaml
  label: scope-bid Dispatches API
  slug: scope-bid-dispatches-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/scope-bid/openapi/scope-bid-dispatches-api-openapi.yml
- filename: scope-bid-exports-api-openapi.yml
  format: yaml
  label: scope-bid Exports API
  slug: scope-bid-exports-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/scope-bid/openapi/scope-bid-exports-api-openapi.yml
- filename: scope-bid-insights-api-openapi.yml
  format: yaml
  label: scope-bid Insights API
  slug: scope-bid-insights-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/scope-bid/openapi/scope-bid-insights-api-openapi.yml
- filename: scope-bid-matters-api-openapi.yml
  format: yaml
  label: scope-bid Matters API
  slug: scope-bid-matters-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/scope-bid/openapi/scope-bid-matters-api-openapi.yml
- filename: scope-bid-partner-authorizations-api-openapi.yml
  format: yaml
  label: scope-bid Partner Authorizations API
  slug: scope-bid-partner-authorizations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/scope-bid/openapi/scope-bid-partner-authorizations-api-openapi.yml
- filename: scope-bid-scopes-api-openapi.yml
  format: yaml
  label: scope-bid Scopes API
  slug: scope-bid-scopes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/scope-bid/openapi/scope-bid-scopes-api-openapi.yml
- filename: scope-bid-vendors-api-openapi.yml
  format: yaml
  label: scope-bid Vendors API
  slug: scope-bid-vendors-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/scope-bid/openapi/scope-bid-vendors-api-openapi.yml
- filename: scope-bid-webhooks-api-openapi.yml
  format: yaml
  label: scope-bid Webhooks API
  slug: scope-bid-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/scope-bid/openapi/scope-bid-webhooks-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: scope.bid
  spf: true
hosts:
- cert_expires: Dec  4 23:18:15 2026 GMT
  host: scope.bid
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Scope Bid Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for scope-bid, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: scope-bid
provider_slug: scope-bid
slug: scope-bid-domain-security
source_filename: scope-bid-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: scope.bid\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  4 23:18:15 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: scope.bid\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/scope-bid/security/scope-bid-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Construction
- Bidding
- SaaS
- Collaboration
- Analytics
---
