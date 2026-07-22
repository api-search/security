---
api_specs:
- filename: toqio-accounts-openapi.yml
  format: yaml
  label: Toqio Accounts API
  slug: toqio-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/toqio/refs/heads/main/openapi/toqio-accounts-openapi.yml
- filename: toqio-cards-openapi.yml
  format: yaml
  label: Toqio Cards API
  slug: toqio-cards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/toqio/refs/heads/main/openapi/toqio-cards-openapi.yml
- filename: toqio-transactions-openapi.yml
  format: yaml
  label: Toqio Transactions API
  slug: toqio-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/toqio/refs/heads/main/openapi/toqio-transactions-openapi.yml
- filename: toqio-beneficiaries-openapi.yml
  format: yaml
  label: Toqio Beneficiaries API
  slug: toqio-beneficiaries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/toqio/refs/heads/main/openapi/toqio-beneficiaries-openapi.yml
- filename: toqio-fees-openapi.yml
  format: yaml
  label: Toqio Fees API
  slug: toqio-fees-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/toqio/refs/heads/main/openapi/toqio-fees-openapi.yml
- filename: toqio-clients-openapi.yml
  format: yaml
  label: Toqio Clients API
  slug: toqio-clients-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/toqio/refs/heads/main/openapi/toqio-clients-openapi.yml
- filename: toqio-compliance-endpoints-openapi.yml
  format: yaml
  label: Toqio Compliance API
  slug: toqio-compliance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/toqio/refs/heads/main/openapi/toqio-compliance-endpoints-openapi.yml
- filename: toqio-upload-kyb-documents-openapi.yml
  format: yaml
  label: Toqio KYB Documents API
  slug: toqio-kyb-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/toqio/refs/heads/main/openapi/toqio-upload-kyb-documents-openapi.yml
- filename: toqio-create-lead-service-openapi.yml
  format: yaml
  label: Toqio Create Lead API
  slug: toqio-create-lead-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/toqio/refs/heads/main/openapi/toqio-create-lead-service-openapi.yml
- filename: toqio-revenue-collections-openapi.yml
  format: yaml
  label: Toqio Revenue Collections API
  slug: toqio-revenue-collections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/toqio/refs/heads/main/openapi/toqio-revenue-collections-openapi.yml
- filename: toqio-custom-notifications-openapi.yml
  format: yaml
  label: Toqio Custom Notifications API
  slug: toqio-custom-notifications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/toqio/refs/heads/main/openapi/toqio-custom-notifications-openapi.yml
- filename: toqio-security-openapi.yml
  format: yaml
  label: Toqio Security API
  slug: toqio-security-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/toqio/refs/heads/main/openapi/toqio-security-openapi.yml
- filename: toqio-integration-hub-api-openapi.yml
  format: yaml
  label: Toqio Integration Hub API
  slug: toqio-integration-hub-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/toqio/refs/heads/main/openapi/toqio-integration-hub-api-openapi.yml
- filename: toqio-card-management-api-openapi.yml
  format: yaml
  label: Toqio Card Management API (Integration Hub)
  slug: toqio-card-management-api-integration-hub
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/toqio/refs/heads/main/openapi/toqio-card-management-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: toq.io
  spf: true
hosts:
- cert_expires: Sep 21 23:59:59 2026 GMT
  host: api.sandbox.toq.io
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan  2 23:59:59 2027 GMT
  host: api.toq.io
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 21 23:59:59 2026 GMT
  host: core.sandbox.toq.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Toqio Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Toqio, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Toqio
provider_slug: toqio
slug: toqio-domain-security
source_filename: toqio-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: api.sandbox.toq.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 23:59:59 2026 GMT\n  hsts: null\n- host: api.toq.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  2 23:59:59 2027 GMT\n  hsts: null\n- host: core.sandbox.toq.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: toq.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/toqio/refs/heads/main/security/toqio-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Embedded Finance
- Fintech
- Banking as a Service
- Payments
- Cards
- Corporate Banking
- Lending
- Compliance
- SMEs
---
