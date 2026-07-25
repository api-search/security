---
api_specs:
- filename: highnote-graphql-api-openapi.yml
  format: yaml
  label: Highnote Issuing API
  slug: highnote-issuing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/highnote/refs/heads/main/openapi/highnote-graphql-api-openapi.yml
- filename: highnote-graphql-api-openapi.yml
  format: yaml
  label: Highnote Account Holders & Onboarding API
  slug: highnote-account-holders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/highnote/refs/heads/main/openapi/highnote-graphql-api-openapi.yml
- filename: highnote-graphql-api-openapi.yml
  format: yaml
  label: Highnote Acquiring API
  slug: highnote-acquiring-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/highnote/refs/heads/main/openapi/highnote-graphql-api-openapi.yml
- filename: highnote-graphql-api-openapi.yml
  format: yaml
  label: Highnote Money Movement API
  slug: highnote-money-movement-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/highnote/refs/heads/main/openapi/highnote-graphql-api-openapi.yml
- filename: highnote-graphql-api-openapi.yml
  format: yaml
  label: Highnote Transactions & Disputes API
  slug: highnote-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/highnote/refs/heads/main/openapi/highnote-graphql-api-openapi.yml
- filename: highnote-graphql-api-openapi.yml
  format: yaml
  label: Highnote Spend Controls & Collaborative Authorization API
  slug: highnote-spend-controls-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/highnote/refs/heads/main/openapi/highnote-graphql-api-openapi.yml
- filename: highnote-graphql-api-openapi.yml
  format: yaml
  label: Highnote Webhooks & Event Notifications API
  slug: highnote-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/highnote/refs/heads/main/openapi/highnote-graphql-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: highnote.com
  spf: true
hosts:
- cert_expires: Oct  5 16:00:10 2026 GMT
  host: highnote.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 19 07:12:41 2026 GMT
  host: docs.highnote.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  8 03:18:20 2026 GMT
  host: api.us.highnote.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Highnote Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Highnote, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Highnote
provider_slug: highnote
slug: highnote-domain-security
source_filename: highnote-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: highnote.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 16:00:10 2026 GMT\n  hsts: null\n- host: docs.highnote.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 19 07:12:41 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.us.highnote.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 03:18:20 2026 GMT\n  hsts: null\ndomains:\n- domain: highnote.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/highnote/refs/heads/main/security/highnote-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Card Issuing
- Card Acquiring
- Embedded Finance
- Banking-as-a-Service
- Fintech
- Payments
- GraphQL
- Ledger
- Credit
- Money Movement
- ACH
- KYC
- United States
---
