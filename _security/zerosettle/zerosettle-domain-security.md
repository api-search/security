---
api_specs:
- filename: zerosettle-openapi.json
  format: json
  label: ZeroSettle IAP API
  slug: zerosettle-iap-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zerosettle/refs/heads/main/openapi/zerosettle-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: zerosettle.io
  spf: true
hosts:
- cert_expires: Oct 17 04:26:06 2026 GMT
  host: api.zerosettle.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Zerosettle Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ZeroSettle, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: ZeroSettle
provider_slug: zerosettle
slug: zerosettle-domain-security
source_filename: zerosettle-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: api.zerosettle.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 17 04:26:06 2026 GMT\n  hsts: null\ndomains:\n- domain: zerosettle.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zerosettle/refs/heads/main/security/zerosettle-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Payments
- In-App Purchase
- Subscriptions
- Merchant of Record
- Billing
- Mobile
- Developer Tools
---
