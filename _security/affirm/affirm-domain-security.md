---
api_specs:
- filename: affirm-transactions-api-openapi.yml
  format: yaml
  label: Affirm Transactions API
  slug: affirm-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/affirm/refs/heads/main/openapi/affirm-transactions-api-openapi.yml
- filename: affirm-authorization-api-openapi.yml
  format: yaml
  label: Affirm Authorization API
  slug: affirm-authorization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/affirm/refs/heads/main/openapi/affirm-authorization-api-openapi.yml
- filename: affirm-cards-api-openapi.yml
  format: yaml
  label: Affirm Cards API
  slug: affirm-cards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/affirm/refs/heads/main/openapi/affirm-cards-api-openapi.yml
- filename: affirm-checkouts-api-openapi.yml
  format: yaml
  label: Affirm Checkouts API
  slug: affirm-checkouts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/affirm/refs/heads/main/openapi/affirm-checkouts-api-openapi.yml
- filename: affirm-disputes-api-openapi.yml
  format: yaml
  label: Affirm Disputes API
  slug: affirm-disputes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/affirm/refs/heads/main/openapi/affirm-disputes-api-openapi.yml
- filename: affirm-promos-api-openapi.yml
  format: yaml
  label: Affirm Promos API
  slug: affirm-promos-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/affirm/refs/heads/main/openapi/affirm-promos-api-openapi.yml
- filename: affirm-settlement-events-api-openapi.yml
  format: yaml
  label: Affirm Settlement Events API
  slug: affirm-settlement-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/affirm/refs/heads/main/openapi/affirm-settlement-events-api-openapi.yml
- filename: affirm-transaction-events-api-openapi.yml
  format: yaml
  label: Affirm Transaction Events API
  slug: affirm-transaction-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/affirm/refs/heads/main/openapi/affirm-transaction-events-api-openapi.yml
- filename: affirm-transactions-api-openapi.yml
  format: yaml
  label: Affirm Transactions API
  slug: affirm-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/affirm/refs/heads/main/openapi/affirm-transactions-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: affirm.com
  spf: true
hosts:
- cert_expires: Sep  9 05:58:42 2026 GMT
  host: www.affirm.com
  hsts: true
  hsts_max_age: 31557600
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  2 14:18:10 2026 GMT
  host: docs.affirm.com
  hsts: true
  hsts_max_age: 31557600
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  9 05:58:42 2026 GMT
  host: api.affirm.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Affirm Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Affirm, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Affirm
provider_slug: affirm
slug: affirm-domain-security
source_filename: affirm-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.affirm.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  9 05:58:42 2026 GMT\n  hsts: true\n  hsts_max_age: 31557600\n- host: docs.affirm.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 14:18:10 2026 GMT\n  hsts: true\n  hsts_max_age: 31557600\n- host: api.affirm.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  9 05:58:42 2026 GMT\n  hsts: null\ndomains:\n- domain: affirm.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/affirm/refs/heads/main/security/affirm-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Fintech
- BNPL
- Lending
- Payments
- Consumer
---
