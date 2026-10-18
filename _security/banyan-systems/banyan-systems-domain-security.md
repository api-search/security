---
api_specs:
- filename: banyan-systems-authentication-api-openapi.yml
  format: yaml
  label: Banyan Systems Authentication API
  slug: banyan-systems-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/banyan-systems/refs/heads/main/openapi/banyan-systems-authentication-api-openapi.yml
- filename: banyan-systems-card-linked-offer-api-openapi.yml
  format: yaml
  label: Banyan Systems Card Linked Offer API
  slug: banyan-systems-card-linked-offer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/banyan-systems/refs/heads/main/openapi/banyan-systems-card-linked-offer-api-openapi.yml
- filename: banyan-systems-consent-api-openapi.yml
  format: yaml
  label: Banyan Systems Consent API
  slug: banyan-systems-consent-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/banyan-systems/refs/heads/main/openapi/banyan-systems-consent-api-openapi.yml
- filename: banyan-systems-enriched-data-api-openapi.yml
  format: yaml
  label: Banyan Systems Enriched Data API
  slug: banyan-systems-enriched-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/banyan-systems/refs/heads/main/openapi/banyan-systems-enriched-data-api-openapi.yml
- filename: banyan-systems-enriched-data-merchant-service-provider-api-openapi.yml
  format: yaml
  label: Banyan Systems Enriched Data - Merchant Service Provider API
  slug: banyan-systems-enriched-data-merchant-service-provider-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/banyan-systems/refs/heads/main/openapi/banyan-systems-enriched-data-merchant-service-provider-api-openapi.yml
- filename: banyan-systems-history-api-openapi.yml
  format: yaml
  label: Banyan Systems History API
  slug: banyan-systems-history-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/banyan-systems/refs/heads/main/openapi/banyan-systems-history-api-openapi.yml
- filename: banyan-systems-receipt-api-openapi.yml
  format: yaml
  label: Banyan Systems Receipt API
  slug: banyan-systems-receipt-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/banyan-systems/refs/heads/main/openapi/banyan-systems-receipt-api-openapi.yml
- filename: banyan-systems-tag-counter-api-openapi.yml
  format: yaml
  label: Banyan Systems Tag Counter API
  slug: banyan-systems-tag-counter-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/banyan-systems/refs/heads/main/openapi/banyan-systems-tag-counter-api-openapi.yml
- filename: banyan-systems-transaction-api-openapi.yml
  format: yaml
  label: Banyan Systems Transaction API
  slug: banyan-systems-transaction-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/banyan-systems/refs/heads/main/openapi/banyan-systems-transaction-api-openapi.yml
- filename: banyan-systems-webhook-api-openapi.yml
  format: yaml
  label: Banyan Systems Webhook API
  slug: banyan-systems-webhook-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/banyan-systems/refs/heads/main/openapi/banyan-systems-webhook-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: banyan.com
  spf: true
hosts:
- cert_expires: Aug 23 06:26:40 2026 GMT
  host: developers.banyan.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 29 08:57:49 2026 GMT
  host: api.banyan.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: Banyan Systems Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Banyan Systems, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Banyan Systems
provider_slug: banyan-systems
slug: banyan-systems-domain-security
source_filename: banyan-systems-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developers.banyan.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 23 06:26:40 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.banyan.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 29 08:57:49 2026 GMT\n  hsts: false\ndomains:\n- domain: banyan.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/banyan-systems/refs/heads/main/security/banyan-systems-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Receipt Data
- Transaction Enrichment
- Item-Level Data
- Card-Linked Offers
- Fintech
- Payments
- Data Collaboration
- Webhook
- Data Enrichment
---
