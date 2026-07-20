---
api_specs:
- filename: qonto-openapi.yml
  format: yaml
  label: Qonto Business API
  slug: qonto-business-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qonto/refs/heads/main/openapi/qonto-openapi.yml
- filename: qonto-openapi.yml
  format: yaml
  label: Qonto Transactions & Statements API
  slug: qonto-transactions-statements-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qonto/refs/heads/main/openapi/qonto-openapi.yml
- filename: qonto-openapi.yml
  format: yaml
  label: Qonto SEPA Transfers API
  slug: qonto-sepa-transfers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qonto/refs/heads/main/openapi/qonto-openapi.yml
- filename: qonto-openapi.yml
  format: yaml
  label: Qonto International Transfers API
  slug: qonto-international-transfers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qonto/refs/heads/main/openapi/qonto-openapi.yml
- filename: qonto-openapi.yml
  format: yaml
  label: Qonto Internal Transfers API
  slug: qonto-internal-transfers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qonto/refs/heads/main/openapi/qonto-openapi.yml
- filename: qonto-openapi.yml
  format: yaml
  label: Qonto Cards API
  slug: qonto-cards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qonto/refs/heads/main/openapi/qonto-openapi.yml
- filename: qonto-openapi.yml
  format: yaml
  label: Qonto Client Invoices & Quotes API
  slug: qonto-client-invoices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qonto/refs/heads/main/openapi/qonto-openapi.yml
- filename: qonto-openapi.yml
  format: yaml
  label: Qonto Supplier Invoices API
  slug: qonto-supplier-invoices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qonto/refs/heads/main/openapi/qonto-openapi.yml
- filename: qonto-openapi.yml
  format: yaml
  label: Qonto SEPA Direct Debit API
  slug: qonto-sepa-direct-debit-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qonto/refs/heads/main/openapi/qonto-openapi.yml
- filename: qonto-openapi.yml
  format: yaml
  label: Qonto Payment Links API
  slug: qonto-payment-links-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qonto/refs/heads/main/openapi/qonto-openapi.yml
- filename: qonto-openapi.yml
  format: yaml
  label: Qonto Terminals API
  slug: qonto-terminals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qonto/refs/heads/main/openapi/qonto-openapi.yml
- filename: qonto-openapi.yml
  format: yaml
  label: Qonto Webhooks API
  slug: qonto-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qonto/refs/heads/main/openapi/qonto-openapi.yml
- filename: qonto-openapi.yml
  format: yaml
  label: Qonto Onboarding API
  slug: qonto-onboarding-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qonto/refs/heads/main/openapi/qonto-openapi.yml
- filename: qonto-openapi.yml
  format: yaml
  label: Qonto Embed SDK & Hosted Pages API
  slug: qonto-embed-sdk-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qonto/refs/heads/main/openapi/qonto-openapi.yml
description: ''
domains:
- dmarc: true
  dmarc_policy: reject
  dmarc_record: v=DMARC1; p=reject; rua=mailto:dmarc_agg@vali.email
  domain: qonto.com
  spf: true
  spf_record: v=spf1 include:_spf.google.com include:sendgrid.net include:amazonses.com include:_spf.salesforce.com include:mail.zendesk.com ~all
hosts:
- host: qonto.com
  hsts: null
  https: true
  note: Marketing site fronted by CloudFront; redirects (301) to canonical host.
  server: CloudFront
  tls_version: TLSv1.3
- host: thirdparty.qonto.com
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 315360000
  hsts_preload: true
  http_version: HTTP/2
  https: true
  note: Production Business API host; unauthenticated request returns HTTP 400.
  server: cloudflare
  tls_version: TLSv1.2
- host: docs.qonto.com
  hsts: null
  https: true
  note: Developer documentation (Mintlify-style, llms.txt published).
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Qonto Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Qonto, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Qonto
provider_slug: qonto
slug: qonto-domain-security
source_filename: qonto-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + docs/API hosts\nhosts:\n- host: qonto.com\n  https: true\n  tls_version: TLSv1.3\n  server: CloudFront\n  hsts: null\n  note: Marketing site fronted by CloudFront; redirects (301) to canonical host.\n- host: thirdparty.qonto.com\n  https: true\n  http_version: HTTP/2\n  tls_version: TLSv1.2\n  server: cloudflare\n  hsts: true\n  hsts_max_age: 315360000\n  hsts_include_subdomains: true\n  hsts_preload: true\n  note: Production Business API host; unauthenticated request returns HTTP 400.\n- host: docs.qonto.com\n  https: true\n  tls_version: TLSv1.3\n  hsts: null\n  note: Developer documentation (Mintlify-style, llms.txt published).\ndomains:\n- domain: qonto.com\n  spf: true\n  spf_record: v=spf1 include:_spf.google.com include:sendgrid.net include:amazonses.com include:_spf.salesforce.com include:mail.zendesk.com ~all\n  dmarc: true\n  dmarc_policy: reject\n  dmarc_record: v=DMARC1; p=reject;\
  \ rua=mailto:dmarc_agg@vali.email\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/qonto/refs/heads/main/security/qonto-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Business Banking
- Neobank
- Fintech
- Payments
- SEPA
- Open Banking
- EUR
- Europe
---
