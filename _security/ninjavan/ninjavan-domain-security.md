---
api_specs:
- filename: ninjavan-oauth-api-api-openapi.yml
  format: yaml
  label: Ninja Van OAuth API
  slug: ninjavan-oauth-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ninjavan/refs/heads/main/openapi/ninjavan-oauth-api-api-openapi.yml
- filename: ninjavan-order-api-api-openapi.yml
  format: yaml
  label: Ninja Van Order API
  slug: ninjavan-order-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ninjavan/refs/heads/main/openapi/ninjavan-order-api-api-openapi.yml
- filename: ninjavan-pudo-api-api-openapi.yml
  format: yaml
  label: Ninja Van PUDO API
  slug: ninjavan-pudo-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ninjavan/refs/heads/main/openapi/ninjavan-pudo-api-api-openapi.yml
- filename: ninjavan-tariff-api-api-openapi.yml
  format: yaml
  label: Ninja Van Tariff API
  slug: ninjavan-tariff-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ninjavan/refs/heads/main/openapi/ninjavan-tariff-api-api-openapi.yml
- filename: ninjavan-tracking-api-api-openapi.yml
  format: yaml
  label: Ninja Van Tracking API
  slug: ninjavan-tracking-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ninjavan/refs/heads/main/openapi/ninjavan-tracking-api-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: ninjavan.co
  spf: true
hosts:
- cert_expires: Jan  1 00:56:46 2027 GMT
  host: www.ninjavan.co
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 22 21:31:23 2026 GMT
  host: api-docs.ninjavan.co
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: Ninjavan Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ninja Van, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Ninja Van
provider_slug: ninjavan
slug: ninjavan-domain-security
source_filename: ninjavan-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-08'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.ninjavan.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  1 00:56:46 2027 GMT\n  hsts: null\n- host: api-docs.ninjavan.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 22 21:31:23 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: ninjavan.co\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ninjavan/refs/heads/main/security/ninjavan-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Logistics
- Last Mile Delivery
- Shipping
- Southeast Asia
- Parcel
- Tracking
- Fulfillment
- E-commerce Logistics
- Waybill
- Software-as-a-Service
---
