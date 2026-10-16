---
api_specs:
- filename: qrx-openapi-generated.yml
  format: yaml
  label: QRX API
  slug: qrx-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qrx/refs/heads/main/openapi/_ae-authored/qrx-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: qrx.codes
  spf: true
hosts:
- cert_expires: Apr  7 23:59:59 2027 GMT
  host: qrx.codes
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Qrx Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for QRX, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: QRX
provider_slug: qrx
slug: qrx-domain-security
source_filename: qrx-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: qrx.codes\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Apr  7 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: qrx.codes\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/qrx/refs/heads/main/security/qrx-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- QR code
- AI
- Art
- API
---
