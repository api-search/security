---
api_specs:
- filename: payhip-openapi.yml
  format: yaml
  label: Payhip Coupons API
  slug: payhip-coupons-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/payhip/refs/heads/main/openapi/payhip-openapi.yml
- filename: payhip-openapi.yml
  format: yaml
  label: Payhip License Keys API
  slug: payhip-license-keys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/payhip/refs/heads/main/openapi/payhip-openapi.yml
- filename: payhip-openapi.yml
  format: yaml
  label: Payhip Webhooks API
  slug: payhip-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/payhip/refs/heads/main/openapi/payhip-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: payhip.com
  spf: true
hosts:
- cert_expires: Aug 14 02:56:54 2026 GMT
  host: payhip.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 27 18:18:41 2026 GMT
  host: help.payhip.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Payhip Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Payhip, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Payhip
provider_slug: payhip
slug: payhip-domain-security
source_filename: payhip-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: payhip.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 14 02:56:54 2026 GMT\n  hsts: false\n- host: help.payhip.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 27 18:18:41 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: payhip.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/payhip/refs/heads/main/security/payhip-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- E-commerce
- Digital Products
- Memberships
- Creators
- Coupons
- License Keys
- Webhooks
- Payments
---
