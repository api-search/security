---
api_specs:
- filename: dojo-api.json
  format: json
  label: Dojo API
  slug: dojo-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dojo/refs/heads/main/openapi/dojo-api.json
- filename: dojo-transactions-api.json
  format: json
  label: Dojo Transaction API
  slug: dojo-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dojo/refs/heads/main/openapi/dojo-transactions-api.json
- filename: dojo-epos-data-api.json
  format: json
  label: Dojo EPOS Data API
  slug: dojo-epos-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dojo/refs/heads/main/openapi/dojo-epos-data-api.json
- filename: dojo-tap-to-pay-on-iphone-api.json
  format: json
  label: Dojo Tap to Pay on iPhone API
  slug: dojo-tap-to-pay-on-iphone-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dojo/refs/heads/main/openapi/dojo-tap-to-pay-on-iphone-api.json
- filename: dojo-epos-tester-tool-api.json
  format: json
  label: Dojo EPOS Tester Tool API
  slug: dojo-epos-tester-tool-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dojo/refs/heads/main/openapi/dojo-epos-tester-tool-api.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: dojo.tech
  spf: true
hosts:
- cert_expires: Sep 20 09:07:11 2026 GMT
  host: dojo.tech
  hsts: true
  hsts_max_age: 0
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  3 23:59:59 2026 GMT
  host: docs.dojo.tech
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  3 23:59:59 2026 GMT
  host: api.dojo.tech
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Dojo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Dojo, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Dojo
provider_slug: dojo
slug: dojo-domain-security
source_filename: dojo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-24'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: dojo.tech\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 09:07:11 2026 GMT\n  hsts: true\n  hsts_max_age: 0\n- host: docs.dojo.tech\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  3 23:59:59 2026 GMT\n  hsts: false\n- host: api.dojo.tech\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  3 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: dojo.tech\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dojo/refs/heads/main/security/dojo-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Payments
- United Kingdom
- Payment Gateway
- Payment Processing
- Acquiring
- Card Payments
- In-Person Payments
- Terminals
- Point-of-Sale
- Webhook
---
