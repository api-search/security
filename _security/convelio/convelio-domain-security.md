---
api_specs:
- filename: convelio-shipping-api-openapi.yml
  format: yaml
  label: Convelio Shipping API
  slug: convelio-shipping-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/convelio/refs/heads/main/openapi/convelio-shipping-api-openapi.yml
- filename: convelio-webhook-api-openapi.yml
  format: yaml
  label: Convelio Webhook API
  slug: convelio-webhook-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/convelio/refs/heads/main/openapi/convelio-webhook-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: convelio.com
  spf: true
hosts:
- cert_expires: Oct  3 07:53:19 2026 GMT
  host: www.convelio.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  2 00:13:09 2026 GMT
  host: developers.convelio.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 22 11:33:33 2026 GMT
  host: api.convelio.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Convelio Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Convelio, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Convelio
provider_slug: convelio
slug: convelio-domain-security
source_filename: convelio-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-09'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.convelio.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 07:53:19 2026 GMT\n  hsts: false\n- host: developers.convelio.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  2 00:13:09 2026 GMT\n  hsts: false\n- host: api.convelio.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 22 11:33:33 2026 GMT\n  hsts: null\ndomains:\n- domain: convelio.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/convelio/refs/heads/main/security/convelio-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Logistics
- Shipping
- Fine Art
- Freight
- E-Commerce
- Quotes
- Webhook
- Customs
- Insurance
---
