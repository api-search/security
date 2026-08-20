---
api_specs:
- filename: zubale-api-documentation-for-external-notification-handler-api-openapi.yml
  format: yaml
  label: Zubale API Documentation for External Notification Handler API
  slug: zubale-api-documentation-for-external-notification-handler-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zubale/refs/heads/main/openapi/zubale-api-documentation-for-external-notification-handler-api-openapi.yml
- filename: zubale-cancel-tasks-api-openapi.yml
  format: yaml
  label: Zubale Cancel tasks API
  slug: zubale-cancel-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zubale/refs/heads/main/openapi/zubale-cancel-tasks-api-openapi.yml
- filename: zubale-delivery-api-api-openapi.yml
  format: yaml
  label: Zubale Delivery API API
  slug: zubale-delivery-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zubale/refs/heads/main/openapi/zubale-delivery-api-api-openapi.yml
- filename: zubale-external-outbound-api-openapi.yml
  format: yaml
  label: Zubale External outbound API
  slug: zubale-external-outbound-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zubale/refs/heads/main/openapi/zubale-external-outbound-api-openapi.yml
- filename: zubale-live-tracking-for-cencosud-api-openapi.yml
  format: yaml
  label: Zubale Live Tracking For Cencosud API
  slug: zubale-live-tracking-for-cencosud-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zubale/refs/heads/main/openapi/zubale-live-tracking-for-cencosud-api-openapi.yml
- filename: zubale-picking-delivery-api-api-openapi.yml
  format: yaml
  label: Zubale Picking & Delivery API API
  slug: zubale-picking-delivery-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zubale/refs/heads/main/openapi/zubale-picking-delivery-api-api-openapi.yml
- filename: zubale-product-catalog-api-openapi.yml
  format: yaml
  label: Zubale Product catalog API
  slug: zubale-product-catalog-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zubale/refs/heads/main/openapi/zubale-product-catalog-api-openapi.yml
- filename: zubale-webhook-payload-structure-for-order-notification-api-openapi.yml
  format: yaml
  label: 'Zubale Webhook: Payload Structure for Order Notification API'
  slug: zubale-webhook-payload-structure-for-order-notification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zubale/refs/heads/main/openapi/zubale-webhook-payload-structure-for-order-notification-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: zubale.com
  spf: true
hosts:
- cert_expires: Dec 12 23:59:59 2026 GMT
  host: zubale.com
  hsts: false
  https: true
  tls_version: TLSv1.2
- cert_expires: Dec 12 23:59:59 2026 GMT
  host: api.zubale.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 12 23:59:59 2026 GMT
  host: api-cencosandbox.zubale.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Zubale Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Zubale, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Zubale
provider_slug: zubale
slug: zubale-domain-security
source_filename: zubale-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: zubale.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 12 23:59:59 2026 GMT\n  hsts: false\n- host: api.zubale.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 12 23:59:59 2026 GMT\n  hsts: null\n- host: api-cencosandbox.zubale.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 12 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: zubale.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zubale/refs/heads/main/security/zubale-domain-security.yml
summary_line: TLSv1.2 · DNSSEC · DMARC
tags:
- Company
- E-Commerce
---
