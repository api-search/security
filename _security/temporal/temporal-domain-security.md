---
api_specs:
- filename: temporal-api-keys-api-openapi.yml
  format: yaml
  label: Temporal API Keys API
  slug: temporal-api-keys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/temporal/refs/heads/main/openapi/temporal-api-keys-api-openapi.yml
- filename: temporal-async-operations-api-openapi.yml
  format: yaml
  label: Temporal Async Operations API
  slug: temporal-async-operations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/temporal/refs/heads/main/openapi/temporal-async-operations-api-openapi.yml
- filename: temporal-namespaces-api-openapi.yml
  format: yaml
  label: Temporal Namespaces API
  slug: temporal-namespaces-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/temporal/refs/heads/main/openapi/temporal-namespaces-api-openapi.yml
- filename: temporal-regions-api-openapi.yml
  format: yaml
  label: Temporal Regions API
  slug: temporal-regions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/temporal/refs/heads/main/openapi/temporal-regions-api-openapi.yml
- filename: temporal-service-accounts-api-openapi.yml
  format: yaml
  label: Temporal Service Accounts API
  slug: temporal-service-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/temporal/refs/heads/main/openapi/temporal-service-accounts-api-openapi.yml
- filename: temporal-users-api-openapi.yml
  format: yaml
  label: Temporal Users API
  slug: temporal-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/temporal/refs/heads/main/openapi/temporal-users-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "amazon.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: temporal.io
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: tmprl.cloud
  spf: true
hosts:
- cert_expires: Sep 21 16:02:20 2026 GMT
  host: temporal.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 27 07:02:20 2026 GMT
  host: docs.temporal.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  8 18:39:20 2026 GMT
  host: saas-api.tmprl.cloud
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Temporal Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Temporal, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Temporal
provider_slug: temporal
slug: temporal-domain-security
source_filename: temporal-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: temporal.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 16:02:20 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.temporal.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 27 07:02:20 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: saas-api.tmprl.cloud\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 18:39:20 2026 GMT\n  hsts: null\ndomains:\n- domain: temporal.io\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: tmprl.cloud\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/temporal/refs/heads/main/security/temporal-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Pro-Code-API-Composition
- Workflows
---
