---
api_specs:
- filename: spod-openapi.yml
  format: yaml
  label: SPOD Articles API
  slug: spod-articles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spod/refs/heads/main/openapi/spod-openapi.yml
- filename: spod-openapi.yml
  format: yaml
  label: SPOD Orders API
  slug: spod-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spod/refs/heads/main/openapi/spod-openapi.yml
- filename: spod-openapi.yml
  format: yaml
  label: SPOD Shipping API
  slug: spod-shipping-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spod/refs/heads/main/openapi/spod-openapi.yml
- filename: spod-openapi.yml
  format: yaml
  label: SPOD Product Types API
  slug: spod-product-types-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spod/refs/heads/main/openapi/spod-openapi.yml
- filename: spod-openapi.yml
  format: yaml
  label: SPOD Stock API
  slug: spod-stock-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spod/refs/heads/main/openapi/spod-openapi.yml
- filename: spod-openapi.yml
  format: yaml
  label: SPOD Subscriptions and Webhooks API
  slug: spod-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spod/refs/heads/main/openapi/spod-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "letsencrypt.org"
  - 0 issue "letsencrypt.org"
  - 0 issue "digicert.com"
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: spod.com
  spf: true
- caa:
  - 0 issuewild "letsencrypt.org"
  - 0 issue "letsencrypt.org"
  dmarc: false
  dnssec: false
  domain: spreadconnect-staging.app
  spf: false
hosts:
- cert_expires: Aug 22 15:38:30 2026 GMT
  host: www.spod.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 22 15:38:30 2026 GMT
  host: rest.spod.com
  hsts: true
  hsts_max_age: 15768000
  https: true
  tls_version: TLSv1.3
- host: rest.spreadconnect-staging.app
  https: false
kind: domain-security
layout: security
method: probed
name: Spod Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SPOD, probed live across 3 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: SPOD
provider_slug: spod
slug: spod-domain-security
source_filename: spod-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.spod.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 22 15:38:30 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: rest.spod.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 22 15:38:30 2026 GMT\n  hsts: true\n  hsts_max_age: 15768000\n- host: rest.spreadconnect-staging.app\n  https: false\ndomains:\n- domain: spod.com\n  dnssec: true\n  caa:\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"digicert.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: spreadconnect-staging.app\n  dnssec: false\n  caa:\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issue \"letsencrypt.org\"\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/spod/refs/heads/main/security/spod-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Print on Demand
- POD
- Dropshipping
- Fulfillment
- E-commerce
- Merchandise
- Spreadshirt
- Spreadconnect
---
