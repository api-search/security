---
api_specs:
- filename: emerge-authentication-api-openapi.yml
  format: yaml
  label: Emerge Authentication API
  slug: emerge-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/emerge/refs/heads/main/openapi/emerge-authentication-api-openapi.yml
- filename: emerge-awards-api-openapi.yml
  format: yaml
  label: Emerge Awards API
  slug: emerge-awards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/emerge/refs/heads/main/openapi/emerge-awards-api-openapi.yml
- filename: emerge-network-partners-api-openapi.yml
  format: yaml
  label: Emerge Network Partners API
  slug: emerge-network-partners-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/emerge/refs/heads/main/openapi/emerge-network-partners-api-openapi.yml
- filename: emerge-opportunities-api-openapi.yml
  format: yaml
  label: Emerge Opportunities API
  slug: emerge-opportunities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/emerge/refs/heads/main/openapi/emerge-opportunities-api-openapi.yml
- filename: emerge-options-api-openapi.yml
  format: yaml
  label: Emerge Options API
  slug: emerge-options-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/emerge/refs/heads/main/openapi/emerge-options-api-openapi.yml
- filename: emerge-shipments-api-openapi.yml
  format: yaml
  label: Emerge Shipments API
  slug: emerge-shipments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/emerge/refs/heads/main/openapi/emerge-shipments-api-openapi.yml
- filename: emerge-tender-api-openapi.yml
  format: yaml
  label: Emerge Tender API
  slug: emerge-tender-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/emerge/refs/heads/main/openapi/emerge-tender-api-openapi.yml
- filename: emerge-tenders-api-openapi.yml
  format: yaml
  label: Emerge Tenders API
  slug: emerge-tenders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/emerge/refs/heads/main/openapi/emerge-tenders-api-openapi.yml
- filename: emerge-webhooks-api-openapi.yml
  format: yaml
  label: Emerge Webhooks API
  slug: emerge-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/emerge/refs/heads/main/openapi/emerge-webhooks-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: emergemarket.com
  spf: true
- caa:
  - 0 issuewild "ssl.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: emergemarket.io
  spf: true
hosts:
- cert_expires: Sep 19 20:29:16 2026 GMT
  host: www.emergemarket.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  1 22:31:42 2026 GMT
  host: api-docs.emergemarket.io
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  1 22:31:42 2026 GMT
  host: api.emergemarket.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Emerge Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Emerge, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Emerge
provider_slug: emerge
slug: emerge-domain-security
source_filename: emerge-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.emergemarket.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 19 20:29:16 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api-docs.emergemarket.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 22:31:42 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: api.emergemarket.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 22:31:42 2026 GMT\n  hsts: null\ndomains:\n- domain: emergemarket.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: emergemarket.io\n  dnssec: true\n  caa:\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/emerge/refs/heads/main/security/emerge-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- freight
- Logistics
- Transportation
- Supply Chain
- Procurement
- trucking
- freight-marketplace
- transportation-management
- Shipping
- rate-benchmarking
- Webhook
- b2b-marketplace
---
