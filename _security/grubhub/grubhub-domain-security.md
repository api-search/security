---
api_specs:
- filename: grubhub-delivery-quotes-api-openapi.yml
  format: yaml
  label: Grubhub Delivery Quotes API
  slug: grubhub-delivery-quotes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/grubhub/refs/heads/main/openapi/grubhub-delivery-quotes-api-openapi.yml
- filename: grubhub-delivery-refunds-api-openapi.yml
  format: yaml
  label: Grubhub Delivery Refunds API
  slug: grubhub-delivery-refunds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/grubhub/refs/heads/main/openapi/grubhub-delivery-refunds-api-openapi.yml
- filename: grubhub-delivery-service-areas-api-openapi.yml
  format: yaml
  label: Grubhub Delivery Service Areas API
  slug: grubhub-delivery-service-areas-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/grubhub/refs/heads/main/openapi/grubhub-delivery-service-areas-api-openapi.yml
- filename: grubhub-delivery-status-api-openapi.yml
  format: yaml
  label: Grubhub Delivery Status API
  slug: grubhub-delivery-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/grubhub/refs/heads/main/openapi/grubhub-delivery-status-api-openapi.yml
- filename: grubhub-delivery-tests-api-openapi.yml
  format: yaml
  label: Grubhub Delivery Tests API
  slug: grubhub-delivery-tests-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/grubhub/refs/heads/main/openapi/grubhub-delivery-tests-api-openapi.yml
- filename: grubhub-delivery-updates-api-openapi.yml
  format: yaml
  label: Grubhub Delivery Updates API
  slug: grubhub-delivery-updates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/grubhub/refs/heads/main/openapi/grubhub-delivery-updates-api-openapi.yml
- filename: grubhub-delivery-webhooks-emulation-api-openapi.yml
  format: yaml
  label: Grubhub Delivery Webhooks Emulation API
  slug: grubhub-delivery-webhooks-emulation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/grubhub/refs/heads/main/openapi/grubhub-delivery-webhooks-emulation-api-openapi.yml
- filename: grubhub-endpoints-api-openapi.yml
  format: yaml
  label: Grubhub Endpoints API
  slug: grubhub-endpoints-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/grubhub/refs/heads/main/openapi/grubhub-endpoints-api-openapi.yml
- filename: grubhub-requesting-reports-api-openapi.yml
  format: yaml
  label: Grubhub Requesting Reports API
  slug: grubhub-requesting-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/grubhub/refs/heads/main/openapi/grubhub-requesting-reports-api-openapi.yml
- filename: grubhub-webhooks-api-openapi.yml
  format: yaml
  label: Grubhub Webhooks API
  slug: grubhub-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/grubhub/refs/heads/main/openapi/grubhub-webhooks-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: grubhub.com
  spf: true
hosts:
- cert_expires: Nov 24 01:08:20 2026 GMT
  host: grubhub.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 24 01:08:20 2026 GMT
  host: developer.grubhub.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- host: api.grubhub.com
  https: false
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Grubhub Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Grubhub, probed live across 3 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Grubhub
provider_slug: grubhub
slug: grubhub-domain-security
source_filename: grubhub-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: grubhub.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 24 01:08:20 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.grubhub.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 24 01:08:20 2026 GMT\n  hsts: false\n- host: api.grubhub.com\n  https: false\ndomains:\n- domain: grubhub.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/grubhub/refs/heads/main/security/grubhub-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Food Delivery
- Restaurant
- Marketplace
- Online Ordering
- Point-of-Sale
- Logistics
- Last Mile Delivery
- Menu Management
- Hospitality
- Local Commerce
- Delivery
---
