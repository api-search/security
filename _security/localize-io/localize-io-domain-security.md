---
api_specs:
- filename: localize-io-assets-api-openapi.yml
  format: yaml
  label: Localize.io Assets API
  slug: localize-io-assets-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/localize-io/openapi/localize-io-assets-api-openapi.yml
- filename: localize-io-configuration-api-openapi.yml
  format: yaml
  label: Localize.io Configuration API
  slug: localize-io-configuration-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/localize-io/openapi/localize-io-configuration-api-openapi.yml
- filename: localize-io-costs-api-openapi.yml
  format: yaml
  label: Localize.io Costs API
  slug: localize-io-costs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/localize-io/openapi/localize-io-costs-api-openapi.yml
- filename: localize-io-feedback-api-openapi.yml
  format: yaml
  label: Localize.io Feedback API
  slug: localize-io-feedback-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/localize-io/openapi/localize-io-feedback-api-openapi.yml
- filename: localize-io-jobs-api-openapi.yml
  format: yaml
  label: Localize.io Jobs API
  slug: localize-io-jobs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/localize-io/openapi/localize-io-jobs-api-openapi.yml
- filename: localize-io-linguists-api-openapi.yml
  format: yaml
  label: Localize.io Linguists API
  slug: localize-io-linguists-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/localize-io/openapi/localize-io-linguists-api-openapi.yml
- filename: localize-io-ops-api-openapi.yml
  format: yaml
  label: Localize.io Ops API
  slug: localize-io-ops-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/localize-io/openapi/localize-io-ops-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: localize.io
  spf: true
hosts:
- cert_expires: Jan  2 23:22:56 2027 GMT
  host: localize.io
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Localize.io Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Localize.io, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Localize.io
provider_slug: localize-io
slug: localize-io-domain-security
source_filename: localize-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: localize.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  2 23:22:56 2027 GMT\n  hsts: false\ndomains:\n- domain: localize.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/localize-io/security/localize-io-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Localization
- Translation API
- Human Review
- Translation Memory
- AI Translation
---
