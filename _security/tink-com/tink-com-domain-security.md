---
api_specs:
- filename: tink-oauth-api-openapi.yml
  format: yaml
  label: Tink OAuth API
  slug: tink-oauth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tink-com/refs/heads/main/openapi/tink-oauth-api-openapi.yml
- filename: tink-account-check-api-openapi.yml
  format: yaml
  label: Tink Account Check API
  slug: tink-account-check-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tink-com/refs/heads/main/openapi/tink-account-check-api-openapi.yml
- filename: tink-data-api-openapi.yml
  format: yaml
  label: Tink Data API
  slug: tink-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tink-com/refs/heads/main/openapi/tink-data-api-openapi.yml
- filename: tink-data-enrichment-api-openapi.yml
  format: yaml
  label: Tink Data Enrichment API
  slug: tink-data-enrichment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tink-com/refs/heads/main/openapi/tink-data-enrichment-api-openapi.yml
- filename: tink-payments-api-openapi.yml
  format: yaml
  label: Tink Payments API
  slug: tink-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tink-com/refs/heads/main/openapi/tink-payments-api-openapi.yml
- filename: tink-risk-reports-api-openapi.yml
  format: yaml
  label: Tink Risk and Reports API
  slug: tink-risk-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tink-com/refs/heads/main/openapi/tink-risk-reports-api-openapi.yml
- filename: tink-money-manager-api-openapi.yml
  format: yaml
  label: Tink Money Manager API
  slug: tink-money-manager-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tink-com/refs/heads/main/openapi/tink-money-manager-api-openapi.yml
- filename: tink-connector-api-openapi.yml
  format: yaml
  label: Tink Connector API
  slug: tink-connector-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tink-com/refs/heads/main/openapi/tink-connector-api-openapi.yml
- filename: tink-webhooks-api-openapi.yml
  format: yaml
  label: Tink Webhooks API
  slug: tink-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tink-com/refs/heads/main/openapi/tink-webhooks-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "multicert.com"
  - 0 iodef "mailto:security@tink.se"
  - 0 issue "amazon.com"
  - 0 issue "digicert.com"
  - 0 issue "e-szigno.hu"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: tink.com
  spf: true
hosts:
- cert_expires: Dec 31 23:59:59 2026 GMT
  host: tink.com
  hsts: true
  hsts_max_age: 15724800
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  6 23:59:59 2026 GMT
  host: docs.tink.com
  hsts: true
  hsts_max_age: 15724800
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 30 23:59:59 2026 GMT
  host: api.tink.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Tink Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Tink, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Tink
provider_slug: tink-com
slug: tink-com-domain-security
source_filename: tink-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: tink.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 31 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 15724800\n- host: docs.tink.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 15724800\n- host: api.tink.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 30 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: tink.com\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"multicert.com\"\n  - 0 iodef \"mailto:security@tink.se\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"e-szigno.hu\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tink-com/refs/heads/main/security/tink-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Open Banking
- PSD2
- Payment Initiation
- Account Aggregation
- Risk Decisioning
- Pay by Bank
- Finance
- Banking
- Europe
- Visa
---
