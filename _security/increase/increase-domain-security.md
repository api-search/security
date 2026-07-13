---
api_specs:
- filename: increase-openapi.json
  format: json
  label: Increase ACH API
  slug: increase-ach-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/increase/refs/heads/main/openapi/increase-openapi.json
- filename: increase-openapi.json
  format: json
  label: Increase Wire Transfers API
  slug: increase-wire-transfers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/increase/refs/heads/main/openapi/increase-openapi.json
- filename: increase-openapi.json
  format: json
  label: Increase Real-Time Payments API
  slug: increase-real-time-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/increase/refs/heads/main/openapi/increase-openapi.json
- filename: increase-openapi.json
  format: json
  label: Increase Check API
  slug: increase-check-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/increase/refs/heads/main/openapi/increase-openapi.json
- filename: increase-openapi.json
  format: json
  label: Increase Cards API
  slug: increase-cards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/increase/refs/heads/main/openapi/increase-openapi.json
- filename: increase-openapi.json
  format: json
  label: Increase Accounts API
  slug: increase-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/increase/refs/heads/main/openapi/increase-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: increase.com
  spf: true
hosts:
- cert_expires: Sep 17 00:37:53 2026 GMT
  host: increase.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 26 03:41:37 2026 GMT
  host: api.increase.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 24 12:59:59 2026 GMT
  host: sandbox.increase.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Increase Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Increase, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Increase
provider_slug: increase
slug: increase-domain-security
source_filename: increase-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: increase.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 17 00:37:53 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.increase.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 03:41:37 2026 GMT\n  hsts: null\n- host: sandbox.increase.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 12:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: increase.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/increase/refs/heads/main/security/increase-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Fintech
- Banking
- Payments
- ACH
- Wires
---
