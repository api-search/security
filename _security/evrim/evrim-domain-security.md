---
api_specs:
- filename: evrim-answers-api-openapi.yml
  format: yaml
  label: Evrim answers API
  slug: evrim-answers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/evrim/refs/heads/main/openapi/evrim-answers-api-openapi.yml
- filename: evrim-blank-api-openapi.yml
  format: yaml
  label: Evrim blank API
  slug: evrim-blank-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/evrim/refs/heads/main/openapi/evrim-blank-api-openapi.yml
- filename: evrim-bulk-api-openapi.yml
  format: yaml
  label: Evrim bulk API
  slug: evrim-bulk-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/evrim/refs/heads/main/openapi/evrim-bulk-api-openapi.yml
- filename: evrim-collections-api-openapi.yml
  format: yaml
  label: Evrim collections API
  slug: evrim-collections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/evrim/refs/heads/main/openapi/evrim-collections-api-openapi.yml
- filename: evrim-compose-api-openapi.yml
  format: yaml
  label: Evrim compose API
  slug: evrim-compose-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/evrim/refs/heads/main/openapi/evrim-compose-api-openapi.yml
- filename: evrim-costs-api-openapi.yml
  format: yaml
  label: Evrim costs API
  slug: evrim-costs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/evrim/refs/heads/main/openapi/evrim-costs-api-openapi.yml
- filename: evrim-created-fields-api-openapi.yml
  format: yaml
  label: Evrim created-fields API
  slug: evrim-created-fields-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/evrim/refs/heads/main/openapi/evrim-created-fields-api-openapi.yml
- filename: evrim-extract-api-openapi.yml
  format: yaml
  label: Evrim extract API
  slug: evrim-extract-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/evrim/refs/heads/main/openapi/evrim-extract-api-openapi.yml
- filename: evrim-fields-api-openapi.yml
  format: yaml
  label: Evrim fields API
  slug: evrim-fields-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/evrim/refs/heads/main/openapi/evrim-fields-api-openapi.yml
- filename: evrim-health-api-openapi.yml
  format: yaml
  label: Evrim health API
  slug: evrim-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/evrim/refs/heads/main/openapi/evrim-health-api-openapi.yml
- filename: evrim-prod-api-openapi.yml
  format: yaml
  label: Evrim prod API
  slug: evrim-prod-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/evrim/refs/heads/main/openapi/evrim-prod-api-openapi.yml
- filename: evrim-profiles-api-openapi.yml
  format: yaml
  label: Evrim profiles API
  slug: evrim-profiles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/evrim/refs/heads/main/openapi/evrim-profiles-api-openapi.yml
- filename: evrim-prompt-templates-api-openapi.yml
  format: yaml
  label: Evrim prompt-templates API
  slug: evrim-prompt-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/evrim/refs/heads/main/openapi/evrim-prompt-templates-api-openapi.yml
- filename: evrim-questions-api-openapi.yml
  format: yaml
  label: Evrim questions API
  slug: evrim-questions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/evrim/refs/heads/main/openapi/evrim-questions-api-openapi.yml
- filename: evrim-snapshots-api-openapi.yml
  format: yaml
  label: Evrim snapshots API
  slug: evrim-snapshots-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/evrim/refs/heads/main/openapi/evrim-snapshots-api-openapi.yml
- filename: evrim-tags-api-openapi.yml
  format: yaml
  label: Evrim tags API
  slug: evrim-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/evrim/refs/heads/main/openapi/evrim-tags-api-openapi.yml
- filename: evrim-templates-api-openapi.yml
  format: yaml
  label: Evrim templates API
  slug: evrim-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/evrim/refs/heads/main/openapi/evrim-templates-api-openapi.yml
- filename: evrim-transform-api-openapi.yml
  format: yaml
  label: Evrim transform API
  slug: evrim-transform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/evrim/refs/heads/main/openapi/evrim-transform-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: evrim.ai
  spf: true
hosts:
- cert_expires: Nov  2 03:54:24 2026 GMT
  host: www.evrim.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- host: docs.evrim.ai
  https: false
- cert_expires: Dec  9 23:59:59 2026 GMT
  host: api.evrim.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Evrim Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Evrim, probed live across 3 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Evrim
provider_slug: evrim
slug: evrim-domain-security
source_filename: evrim-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-14'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.evrim.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  2 03:54:24 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.evrim.ai\n  https: false\n- host: api.evrim.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  9 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: evrim.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/evrim/refs/heads/main/security/evrim-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Intelligence
- Signals
- Data Enrichment
- Profiles
- Entity Resolution
- Defense
- Financial-Services
- Government
---
