---
api_specs:
- filename: openapi
  format: yaml
  label: Mixpanel Ingestion API
  slug: mixpanel-ingestion-api
  spec_type: OpenAPI
  url: https://developer.mixpanel.com/reference/openapi
- filename: openapi
  format: yaml
  label: Mixpanel Query API
  slug: mixpanel-query-api
  spec_type: OpenAPI
  url: https://developer.mixpanel.com/reference/openapi
- filename: openapi
  format: yaml
  label: Mixpanel Data Pipelines API
  slug: mixpanel-data-pipelines-api
  spec_type: OpenAPI
  url: https://developer.mixpanel.com/reference/openapi
- filename: mixpanel-identity-openapi.yml
  format: yaml
  label: Mixpanel Identity API
  slug: mixpanel-identity-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mixpanel/refs/heads/main/openapi/mixpanel-identity-openapi.yml
- filename: mixpanel-event-export-openapi.yml
  format: yaml
  label: Mixpanel Event Export API
  slug: mixpanel-event-export-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mixpanel/refs/heads/main/openapi/mixpanel-event-export-openapi.yml
- filename: mixpanel-lexicon-schemas-openapi.yml
  format: yaml
  label: Mixpanel Lexicon Schemas API
  slug: mixpanel-lexicon-schemas-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mixpanel/refs/heads/main/openapi/mixpanel-lexicon-schemas-openapi.yml
- filename: mixpanel-service-accounts-openapi.yml
  format: yaml
  label: Mixpanel Service Accounts API
  slug: mixpanel-service-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mixpanel/refs/heads/main/openapi/mixpanel-service-accounts-openapi.yml
- filename: mixpanel-annotations-openapi.yml
  format: yaml
  label: Mixpanel Annotations API
  slug: mixpanel-annotations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mixpanel/refs/heads/main/openapi/mixpanel-annotations-openapi.yml
- filename: mixpanel-gdpr-ccpa-openapi.yml
  format: yaml
  label: Mixpanel GDPR and CCPA API
  slug: mixpanel-gdpr-and-ccpa-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mixpanel/refs/heads/main/openapi/mixpanel-gdpr-ccpa-openapi.yml
- filename: mixpanel-warehouse-connectors-openapi.yml
  format: yaml
  label: Mixpanel Warehouse Connectors API
  slug: mixpanel-warehouse-connectors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mixpanel/refs/heads/main/openapi/mixpanel-warehouse-connectors-openapi.yml
- filename: mixpanel-webhooks-asyncapi.yml
  format: yaml
  label: Mixpanel Webhooks
  slug: mixpanel-webhooks
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/mixpanel/refs/heads/main/asyncapi/mixpanel-webhooks-asyncapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: mixpanel.com
  spf: true
hosts:
- cert_expires: Jan 13 23:59:59 2027 GMT
  host: developer.mixpanel.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 13 23:59:59 2027 GMT
  host: api.mixpanel.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 13 23:59:59 2027 GMT
  host: mixpanel.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Mixpanel Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Mixpanel, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Mixpanel
provider_slug: mixpanel
slug: mixpanel-domain-security
source_filename: mixpanel-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developer.mixpanel.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 13 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.mixpanel.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 13 23:59:59 2027 GMT\n  hsts: null\n- host: mixpanel.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 13 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: mixpanel.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mixpanel/refs/heads/main/security/mixpanel-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Analytics
- Data Analysis
- Event Tracking
- Product Analytics
- User Behavior
---
