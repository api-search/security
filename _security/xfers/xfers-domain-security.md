---
api_specs:
- filename: xfers-singapore-openapi.json
  format: json
  label: Xfers Singapore API
  slug: xfers-singapore-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xfers/refs/heads/main/openapi/xfers-singapore-openapi.json
- filename: xfers-indonesia-openapi.json
  format: json
  label: Xfers Indonesia API
  slug: xfers-indonesia-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xfers/refs/heads/main/openapi/xfers-indonesia-openapi.json
- filename: xfers-indonesia-payment-gateway-unique-amount-openapi.json
  format: json
  label: Xfers Indonesia Payment Gateway API
  slug: xfers-indonesia-payment-gateway-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xfers/refs/heads/main/openapi/xfers-indonesia-payment-gateway-unique-amount-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: xfers.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: xfers.io
  spf: true
hosts:
- cert_expires: Oct  5 15:46:00 2026 GMT
  host: xfers.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 23 03:38:06 2026 GMT
  host: docs.xfers.io
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 23 03:38:06 2026 GMT
  host: www.xfers.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Xfers Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Xfers, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Xfers
provider_slug: xfers
slug: xfers-domain-security
source_filename: xfers-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: xfers.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 15:46:00 2026 GMT\n  hsts: null\n- host: docs.xfers.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 23 03:38:06 2026 GMT\n  hsts: false\n- host: www.xfers.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 23 03:38:06 2026 GMT\n  hsts: null\ndomains:\n- domain: xfers.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: xfers.io\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/xfers/refs/heads/main/security/xfers-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Payments
- Fintech
- Bank Transfers
- Digital Wallets
- Lending
- Singapore
- Indonesia
- Southeast Asia
---
