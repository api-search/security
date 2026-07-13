---
api_specs:
- filename: shippo-openapi.yml
  format: yaml
  label: Shippo API
  slug: shippo-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shippo/refs/heads/main/openapi/shippo-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: goshippo.com
  spf: true
hosts:
- cert_expires: Aug 12 10:36:37 2026 GMT
  host: goshippo.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 15 08:43:31 2026 GMT
  host: docs.goshippo.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 25 23:59:59 2026 GMT
  host: api.goshippo.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Shippo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Shippo, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Shippo
provider_slug: shippo
slug: shippo-domain-security
source_filename: shippo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: goshippo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 12 10:36:37 2026 GMT\n  hsts: false\n- host: docs.goshippo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 08:43:31 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.goshippo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 25 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: goshippo.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/shippo/refs/heads/main/security/shippo-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Ecommerce
- Labels
- Logistics
- Returns
- Shipping
- Tracking
---
