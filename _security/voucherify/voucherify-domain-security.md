---
api_specs:
- filename: voucherify-openapi-generated.yml
  format: yaml
  label: Voucherify API
  slug: voucherify-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/voucherify/refs/heads/main/openapi/_ae-authored/voucherify-openapi-generated.yml
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "sectigo.com"
  - 0 iodef "mailto:compliance@voucherify.io"
  - 0 issue "amazon.com"
  - 0 issue "digicert.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: voucherify.io
  spf: true
hosts:
- cert_expires: Dec  5 10:59:22 2026 GMT
  host: www.voucherify.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Voucherify Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Voucherify, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Voucherify
provider_slug: voucherify
slug: voucherify-domain-security
source_filename: voucherify-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-14'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.voucherify.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  5 10:59:22 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: voucherify.io\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"sectigo.com\"\n  - 0 iodef \"mailto:compliance@voucherify.io\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"digicert.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/voucherify/refs/heads/main/security/voucherify-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Incentives
- Promotions
- Loyalty
- API
---
