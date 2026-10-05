---
api_specs:
- filename: qrsalt-barcode-api-openapi.yml
  format: yaml
  label: QRSalt Barcode API
  slug: qrsalt-barcode-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qrsalt/refs/heads/main/openapi/qrsalt-barcode-api-openapi.yml
- filename: qrsalt-codes-api-openapi.yml
  format: yaml
  label: QRSalt Codes API
  slug: qrsalt-codes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qrsalt/refs/heads/main/openapi/qrsalt-codes-api-openapi.yml
- filename: qrsalt-domains-api-openapi.yml
  format: yaml
  label: QRSalt Domains API
  slug: qrsalt-domains-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qrsalt/refs/heads/main/openapi/qrsalt-domains-api-openapi.yml
- filename: qrsalt-forms-api-openapi.yml
  format: yaml
  label: QRSalt Forms API
  slug: qrsalt-forms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qrsalt/refs/heads/main/openapi/qrsalt-forms-api-openapi.yml
- filename: qrsalt-i-api-openapi.yml
  format: yaml
  label: QRSalt I API
  slug: qrsalt-i-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qrsalt/refs/heads/main/openapi/qrsalt-i-api-openapi.yml
- filename: qrsalt-qr-api-openapi.yml
  format: yaml
  label: QRSalt Qr API
  slug: qrsalt-qr-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qrsalt/refs/heads/main/openapi/qrsalt-qr-api-openapi.yml
- filename: qrsalt-qrsalt-api-api-openapi.yml
  format: yaml
  label: QRSalt QRSalt API
  slug: qrsalt-qrsalt-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qrsalt/refs/heads/main/openapi/qrsalt-qrsalt-api-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: qrsalt.com
  spf: true
hosts:
- cert_expires: Dec  8 19:17:15 2026 GMT
  host: qrsalt.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Qrsalt Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for QRSalt, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: QRSalt
provider_slug: qrsalt
slug: qrsalt-domain-security
source_filename: qrsalt-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-03'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: qrsalt.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  8 19:17:15 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: qrsalt.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/qrsalt/refs/heads/main/security/qrsalt-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- QR Codes
- Barcodes
- Analytics
- Dynamic links
---
