---
api_specs:
- filename: osis-co-ai-api-openapi.yml
  format: yaml
  label: osis-co AI API
  slug: osis-co-ai-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/osis-co/openapi/osis-co-ai-api-openapi.yml
- filename: osis-co-calls-api-openapi.yml
  format: yaml
  label: osis-co Calls API
  slug: osis-co-calls-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/osis-co/openapi/osis-co-calls-api-openapi.yml
- filename: osis-co-capabilities-api-openapi.yml
  format: yaml
  label: osis-co Capabilities API
  slug: osis-co-capabilities-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/osis-co/openapi/osis-co-capabilities-api-openapi.yml
- filename: osis-co-conversations-api-openapi.yml
  format: yaml
  label: osis-co Conversations API
  slug: osis-co-conversations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/osis-co/openapi/osis-co-conversations-api-openapi.yml
- filename: osis-co-events-api-openapi.yml
  format: yaml
  label: osis-co Events API
  slug: osis-co-events-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/osis-co/openapi/osis-co-events-api-openapi.yml
- filename: osis-co-groups-api-openapi.yml
  format: yaml
  label: osis-co Groups API
  slug: osis-co-groups-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/osis-co/openapi/osis-co-groups-api-openapi.yml
- filename: osis-co-lines-api-openapi.yml
  format: yaml
  label: osis-co Lines API
  slug: osis-co-lines-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/osis-co/openapi/osis-co-lines-api-openapi.yml
- filename: osis-co-messages-api-openapi.yml
  format: yaml
  label: osis-co Messages API
  slug: osis-co-messages-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/osis-co/openapi/osis-co-messages-api-openapi.yml
- filename: osis-co-number-changes-api-openapi.yml
  format: yaml
  label: osis-co Number Changes API
  slug: osis-co-number-changes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/osis-co/openapi/osis-co-number-changes-api-openapi.yml
- filename: osis-co-payments-api-openapi.yml
  format: yaml
  label: osis-co Payments API
  slug: osis-co-payments-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/osis-co/openapi/osis-co-payments-api-openapi.yml
- filename: osis-co-webhooks-api-openapi.yml
  format: yaml
  label: osis-co Webhooks API
  slug: osis-co-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/osis-co/openapi/osis-co-webhooks-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: osis.co
  spf: true
hosts:
- cert_expires: Dec  8 01:45:12 2026 GMT
  host: osis.co
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Osis Co Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for osis-co, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: osis-co
provider_slug: osis-co
slug: osis-co-domain-security
source_filename: osis-co-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: osis.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  8 01:45:12 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: osis.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/osis-co/security/osis-co-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Messaging
- Communications
- API
- SaaS
- CustomerSupport
---
