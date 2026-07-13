---
api_specs:
- filename: ninjavan-openapi.yml
  format: yaml
  label: Ninja Van OAuth API
  slug: ninjavan-oauth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ninjavan/refs/heads/main/openapi/ninjavan-openapi.yml
- filename: ninjavan-openapi.yml
  format: yaml
  label: Ninja Van Order API
  slug: ninjavan-order-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ninjavan/refs/heads/main/openapi/ninjavan-openapi.yml
- filename: ninjavan-openapi.yml
  format: yaml
  label: Ninja Van Tracking API
  slug: ninjavan-tracking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ninjavan/refs/heads/main/openapi/ninjavan-openapi.yml
- filename: ninjavan-openapi.yml
  format: yaml
  label: Ninja Van Webhooks API
  slug: ninjavan-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ninjavan/refs/heads/main/openapi/ninjavan-openapi.yml
- filename: ninjavan-openapi.yml
  format: yaml
  label: Ninja Van Tariff API
  slug: ninjavan-tariff-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ninjavan/refs/heads/main/openapi/ninjavan-openapi.yml
- filename: ninjavan-openapi.yml
  format: yaml
  label: Ninja Van PUDO API
  slug: ninjavan-pudo-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ninjavan/refs/heads/main/openapi/ninjavan-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: ninjavan.co
  spf: true
  spf_record: v=spf1 include:sendgrid.net include:_spf.google.com include:mail.zendesk.com include:amazonses.com ~all
hosts:
- cert_expires: Jul 31 22:11:52 2026 GMT
  host: ninjavan.co
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Jul 31 22:11:52 2026 GMT
  host: www.ninjavan.co
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  5 11:42:47 2026 GMT
  host: api.ninjavan.co
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jul 31 22:11:52 2026 GMT
  host: aaa.ninjavan.co
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ninjavan Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ninja Van, probed live across 4 host(s) and 1 registrable domain(s). 4 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Ninja Van
provider_slug: ninjavan
slug: ninjavan-domain-security
source_filename: ninjavan-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ninjavan.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jul 31 22:11:52 2026 GMT\n  hsts: false\n- host: www.ninjavan.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jul 31 22:11:52 2026 GMT\n  hsts: false\n- host: api.ninjavan.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 11:42:47 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n  hsts_include_subdomains: true\n- host: aaa.ninjavan.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jul 31 22:11:52 2026 GMT\n  hsts: false\ndomains:\n- domain: ninjavan.co\n  dnssec: true\n  caa: []\n  spf: true\n  spf_record: 'v=spf1 include:sendgrid.net include:_spf.google.com include:mail.zendesk.com include:amazonses.com ~all'\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ninjavan/refs/heads/main/security/ninjavan-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Logistics
- Last-Mile Delivery
- Shipping
- Southeast Asia
- Parcels
- Tracking
- Fulfillment
- E-commerce Logistics
- Waybill
- SaaS
---
