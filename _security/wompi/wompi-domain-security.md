---
api_specs:
- filename: wompi-openapi.yml
  format: yaml
  label: Wompi Transactions API
  slug: wompi-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wompi/refs/heads/main/openapi/wompi-openapi.yml
- filename: wompi-openapi.yml
  format: yaml
  label: Wompi Tokenization API
  slug: wompi-tokenization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wompi/refs/heads/main/openapi/wompi-openapi.yml
- filename: wompi-openapi.yml
  format: yaml
  label: Wompi Payment Sources API
  slug: wompi-payment-sources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wompi/refs/heads/main/openapi/wompi-openapi.yml
- filename: wompi-openapi.yml
  format: yaml
  label: Wompi PSE API
  slug: wompi-pse-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wompi/refs/heads/main/openapi/wompi-openapi.yml
- filename: wompi-openapi.yml
  format: yaml
  label: Wompi Payment Links API
  slug: wompi-payment-links-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wompi/refs/heads/main/openapi/wompi-openapi.yml
- filename: wompi-openapi.yml
  format: yaml
  label: Wompi Merchants & Acceptance Tokens API
  slug: wompi-merchants-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wompi/refs/heads/main/openapi/wompi-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: wompi.co
  notes: SPF via Agari (agari-dns.net). DMARC policy p=reject with aggregate/forensic reporting to bancolombia@rua.agari.com and dmarc@bancolombia.com.co, confirming Grupo Bancolombia operation. No CAA records observed.
  spf: true
hosts:
- cert_expires: Dec 24 23:59:59 2026 GMT
  host: wompi.co
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 31536000
  http_status: 200
  https: true
- cert_expires: Feb 13 23:59:59 2027 GMT
  host: docs.wompi.co
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 31536000
  http_status: 200
  https: true
- cert_expires: Jan 26 23:59:59 2027 GMT
  host: production.wompi.co
  hsts: true
  hsts_max_age: 31536000
  http_status: 403
  https: true
  note: API host; bare requests without a valid bearer key return 403 (expected).
- cert_expires: Jan 26 23:59:59 2027 GMT
  host: sandbox.wompi.co
  hsts: true
  hsts_max_age: 31536000
  http_status: 403
  https: true
  note: Sandbox API host; bare requests without a valid test key return 403 (expected).
kind: domain-security
layout: security
method: probed
name: Wompi Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Wompi, probed live across 4 host(s) and 1 registrable domain(s). 4 host(s) serve HTTPS; 4 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Wompi
provider_slug: wompi
slug: wompi-domain-security
source_filename: wompi-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: wompi.co\n  https: true\n  http_status: 200\n  cert_expires: Dec 24 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n  hsts_include_subdomains: true\n- host: docs.wompi.co\n  https: true\n  http_status: 200\n  cert_expires: Feb 13 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n  hsts_include_subdomains: true\n- host: production.wompi.co\n  https: true\n  http_status: 403\n  cert_expires: Jan 26 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n  note: API host; bare requests without a valid bearer key return 403 (expected).\n- host: sandbox.wompi.co\n  https: true\n  http_status: 403\n  cert_expires: Jan 26 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n  note: Sandbox API host; bare requests without a valid test key return 403 (expected).\ndomains:\n- domain: wompi.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc:\
  \ true\n  dmarc_policy: reject\n  notes: >-\n    SPF via Agari (agari-dns.net). DMARC policy p=reject with aggregate/forensic\n    reporting to bancolombia@rua.agari.com and dmarc@bancolombia.com.co,\n    confirming Grupo Bancolombia operation. No CAA records observed.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wompi/refs/heads/main/security/wompi-domain-security.yml
summary_line: HSTS · DMARC
tags:
- Payments
- Fintech
- Colombia
- LatAm
- Payment Gateway
- PSE
- Nequi
---
