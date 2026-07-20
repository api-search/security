---
api_specs:
- filename: hitchpin-django-api-openapi.json
  format: json
  label: HitchPin Django API (Instant Invoicing)
  slug: hitchpin-django-api-instant-invoicing
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hitchpin/refs/heads/main/openapi/hitchpin-django-api-openapi.json
- filename: hitchpin-receipt-rendering-openapi.json
  format: json
  label: HitchPin Receipt Rendering Service
  slug: hitchpin-receipt-rendering-service
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hitchpin/refs/heads/main/openapi/hitchpin-receipt-rendering-openapi.json
- filename: hitchpin-url-shortener-openapi.json
  format: json
  label: HitchPin URL Shortcode Service
  slug: hitchpin-url-shortcode-service
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hitchpin/refs/heads/main/openapi/hitchpin-url-shortener-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: hitchpin.com
  spf: true
hosts:
- cert_expires: Jan 10 23:59:59 2027 GMT
  host: www.hitchpin.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Hitchpin Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for HitchPin, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: HitchPin
provider_slug: hitchpin
slug: hitchpin-domain-security
source_filename: hitchpin-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.hitchpin.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 10 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: hitchpin.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hitchpin/refs/heads/main/security/hitchpin-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Marketplace
- Agriculture
- Livestock
- Hay and Forage
- Farm Equipment
- Invoicing
- Payments
- Rural
---
