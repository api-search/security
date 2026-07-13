---
api_specs:
- filename: stay-ai-openapi.yml
  format: yaml
  label: Stay AI Subscriptions API
  slug: stay-ai-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stay-ai/refs/heads/main/openapi/stay-ai-openapi.yml
- filename: stay-ai-openapi.yml
  format: yaml
  label: Stay AI Subscription Orders API
  slug: stay-ai-subscription-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stay-ai/refs/heads/main/openapi/stay-ai-openapi.yml
- filename: stay-ai-openapi.yml
  format: yaml
  label: Stay AI Selling Plans API
  slug: stay-ai-selling-plans-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stay-ai/refs/heads/main/openapi/stay-ai-openapi.yml
- filename: stay-ai-openapi.yml
  format: yaml
  label: Stay AI Catalog API
  slug: stay-ai-catalog-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stay-ai/refs/heads/main/openapi/stay-ai-openapi.yml
- filename: stay-ai-openapi.yml
  format: yaml
  label: Stay AI Customer Portal API
  slug: stay-ai-customer-portal-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stay-ai/refs/heads/main/openapi/stay-ai-openapi.yml
- filename: stay-ai-openapi.yml
  format: yaml
  label: Stay AI Webhooks API
  slug: stay-ai-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stay-ai/refs/heads/main/openapi/stay-ai-openapi.yml
- filename: stay-ai-openapi.yml
  format: yaml
  label: Stay AI Account and Data API
  slug: stay-ai-account-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stay-ai/refs/heads/main/openapi/stay-ai-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: stay.ai
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: retextion.com
  spf: true
hosts:
- cert_expires: Sep 19 09:12:32 2026 GMT
  host: stay.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  7 09:49:20 2026 GMT
  host: docs.stay.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  9 23:59:59 2026 GMT
  host: api.retextion.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Stay Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Stay AI, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Stay AI
provider_slug: stay-ai
slug: stay-ai-domain-security
source_filename: stay-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: stay.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 19 09:12:32 2026 GMT\n  hsts: false\n- host: docs.stay.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  7 09:49:20 2026 GMT\n  hsts: null\n- host: api.retextion.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec  9 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: stay.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: retextion.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/stay-ai/refs/heads/main/security/stay-ai-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Subscriptions
- Retention
- Churn
- Shopify
- Ecommerce
- DTC
---
