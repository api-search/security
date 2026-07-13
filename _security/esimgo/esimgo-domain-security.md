---
api_specs:
- filename: esimgo-openapi.yml
  format: yaml
  label: eSIM Go Catalogue API
  slug: catalogue
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/esimgo/refs/heads/main/openapi/esimgo-openapi.yml
- filename: esimgo-openapi.yml
  format: yaml
  label: eSIM Go Orders API
  slug: orders
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/esimgo/refs/heads/main/openapi/esimgo-openapi.yml
- filename: esimgo-openapi.yml
  format: yaml
  label: eSIM Go eSIMs API
  slug: esims
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/esimgo/refs/heads/main/openapi/esimgo-openapi.yml
- filename: esimgo-openapi.yml
  format: yaml
  label: eSIM Go Inventory API
  slug: inventory
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/esimgo/refs/heads/main/openapi/esimgo-openapi.yml
- filename: esimgo-openapi.yml
  format: yaml
  label: eSIM Go Network API
  slug: network
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/esimgo/refs/heads/main/openapi/esimgo-openapi.yml
- filename: esimgo-openapi.yml
  format: yaml
  label: eSIM Go Webhooks
  slug: webhooks
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/esimgo/refs/heads/main/openapi/esimgo-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: esim-go.com
  spf: true
hosts:
- cert_expires: Sep 27 11:41:37 2026 GMT
  host: www.esim-go.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 26 15:15:15 2026 GMT
  host: docs.esim-go.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 30 18:48:04 2026 GMT
  host: api.esim-go.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Esimgo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for eSIM Go, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: eSIM Go
provider_slug: esimgo
slug: esimgo-domain-security
source_filename: esimgo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.esim-go.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 27 11:41:37 2026 GMT\n  hsts: false\n- host: docs.esim-go.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 15:15:15 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: api.esim-go.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 30 18:48:04 2026 GMT\n  hsts: null\ndomains:\n- domain: esim-go.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/esimgo/refs/heads/main/security/esimgo-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- eSIM
- Connectivity
- Travel Data
- Telecom
- Mobile
---
