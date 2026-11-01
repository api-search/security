---
api_specs:
- filename: disban-io-auth-api-openapi.yml
  format: yaml
  label: disban-io Auth API
  slug: disban-io-auth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/disban-io/openapi/disban-io-auth-api-openapi.yml
- filename: disban-io-batch-api-openapi.yml
  format: yaml
  label: disban-io Batch API
  slug: disban-io-batch-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/disban-io/openapi/disban-io-batch-api-openapi.yml
- filename: disban-io-check-api-openapi.yml
  format: yaml
  label: disban-io Check API
  slug: disban-io-check-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/disban-io/openapi/disban-io-check-api-openapi.yml
- filename: disban-io-features-api-openapi.yml
  format: yaml
  label: disban-io Features API
  slug: disban-io-features-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/disban-io/openapi/disban-io-features-api-openapi.yml
- filename: disban-io-keys-api-openapi.yml
  format: yaml
  label: disban-io Keys API
  slug: disban-io-keys-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/disban-io/openapi/disban-io-keys-api-openapi.yml
- filename: disban-io-plans-api-openapi.yml
  format: yaml
  label: disban-io Plans API
  slug: disban-io-plans-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/disban-io/openapi/disban-io-plans-api-openapi.yml
- filename: disban-io-referrals-api-openapi.yml
  format: yaml
  label: disban-io Referrals API
  slug: disban-io-referrals-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/disban-io/openapi/disban-io-referrals-api-openapi.yml
- filename: disban-io-subscription-api-openapi.yml
  format: yaml
  label: disban-io Subscription API
  slug: disban-io-subscription-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/disban-io/openapi/disban-io-subscription-api-openapi.yml
- filename: disban-io-webhooks-api-openapi.yml
  format: yaml
  label: disban-io Webhooks API
  slug: disban-io-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/disban-io/openapi/disban-io-webhooks-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: disban.io
  spf: true
hosts:
- cert_expires: Dec 20 14:30:47 2026 GMT
  host: disban.io
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Disban Io Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for disban-io, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: disban-io
provider_slug: disban-io
slug: disban-io-domain-security
source_filename: disban-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: disban.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 20 14:30:47 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: disban.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/disban-io/security/disban-io-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Email
- Disposable-Email
- API
- Security
- Fraud-Prevention
---
