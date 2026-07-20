---
api_specs:
- filename: holidu-affiliate-api.json
  format: json
  label: Holidu Affiliate API
  slug: holidu-affiliate-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/holidu/refs/heads/main/openapi/holidu-affiliate-api.json
- filename: holidu-connectivity-api.json
  format: json
  label: Holidu Connectivity API
  slug: holidu-connectivity-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/holidu/refs/heads/main/openapi/holidu-connectivity-api.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: holidu.com
  spf: true
hosts:
- cert_expires: Dec 12 23:59:59 2026 GMT
  host: www.holidu.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Holidu Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Holidu, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Holidu
provider_slug: holidu
slug: holidu-domain-security
source_filename: holidu-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.holidu.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 12 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: holidu.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/holidu/refs/heads/main/security/holidu-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Travel And Leisure
- Vacation Rentals
- Short-Term Rentals
- Hospitality
- Property Management
- Booking
- Channel Manager
- Connectivity
- Affiliate
---
