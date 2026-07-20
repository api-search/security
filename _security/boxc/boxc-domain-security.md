---
api_specs:
- filename: boxc-openapi-original.yml
  format: yaml
  label: BoxC API
  slug: boxc-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/boxc/refs/heads/main/openapi/boxc-openapi-original.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: boxc.com
  spf: true
hosts:
- cert_expires: Oct 12 23:59:59 2026 GMT
  host: boxc.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Boxc Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Boxc, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Boxc
provider_slug: boxc
slug: boxc-domain-security
source_filename: boxc-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: boxc.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 12 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: boxc.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/boxc/refs/heads/main/security/boxc-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Logistics
- Shipping
- Ecommerce
- Cross-Border
- Fulfillment
- Customs
- Tracking
- Webhooks
---
