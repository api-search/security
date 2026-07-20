---
api_specs:
- filename: fave-favepay-omni-openapi.yml
  format: yaml
  label: FavePay Omni (FPO) API
  slug: favepay-omni-fpo-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fave/refs/heads/main/openapi/fave-favepay-omni-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: myfave.com
  spf: true
hosts:
- cert_expires: Oct 28 23:59:59 2026 GMT
  host: myfave.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Fave Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Fave, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Fave
provider_slug: fave
slug: fave-domain-security
source_filename: fave-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: myfave.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 28 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: myfave.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fave/refs/heads/main/security/fave-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Payments
- Fintech
- QR Payments
- Loyalty
- Cashback
- Merchant Services
- Southeast Asia
- Webhooks
---
