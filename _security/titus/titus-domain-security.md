---
api_specs:
- filename: titus-authorizations-api-openapi.yml
  format: yaml
  label: Titus Authorizations API
  slug: titus-authorizations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/titus/openapi/titus-authorizations-api-openapi.yml
- filename: titus-businessconnections-api-openapi.yml
  format: yaml
  label: Titus Business Connections API
  slug: titus-businessconnections-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/titus/openapi/titus-businessconnections-api-openapi.yml
- filename: titus-checkouts-api-openapi.yml
  format: yaml
  label: Titus Checkouts API
  slug: titus-checkouts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/titus/openapi/titus-checkouts-api-openapi.yml
- filename: titus-customers-api-openapi.yml
  format: yaml
  label: Titus Customers API
  slug: titus-customers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/titus/openapi/titus-customers-api-openapi.yml
- filename: titus-listings-api-openapi.yml
  format: yaml
  label: Titus Listings API
  slug: titus-listings-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/titus/openapi/titus-listings-api-openapi.yml
- filename: titus-platformpayouts-api-openapi.yml
  format: yaml
  label: Titus Platform Payouts API
  slug: titus-platformpayouts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/titus/openapi/titus-platformpayouts-api-openapi.yml
- filename: titus-refunds-api-openapi.yml
  format: yaml
  label: Titus Refunds API
  slug: titus-refunds-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/titus/openapi/titus-refunds-api-openapi.yml
- filename: titus-titus-api-api-openapi.yml
  format: yaml
  label: Titus Titus API
  slug: titus-titus-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/titus/openapi/titus-titus-api-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: gotitus.com
  spf: true
hosts:
- cert_expires: Jan 20 13:47:30 2027 GMT
  host: www.gotitus.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Titus Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Titus, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Titus
provider_slug: titus
slug: titus-domain-security
source_filename: titus-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.gotitus.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 20 13:47:30 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: gotitus.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/titus/security/titus-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Payments
- FinTech
- Orchestration
- API
- B2B
---
