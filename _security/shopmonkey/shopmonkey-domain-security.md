---
api_specs:
- filename: shopmonkey-openapi.yml
  format: yaml
  label: Shopmonkey Work Orders API
  slug: shopmonkey-work-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shopmonkey/refs/heads/main/openapi/shopmonkey-openapi.yml
- filename: shopmonkey-openapi.yml
  format: yaml
  label: Shopmonkey Customers API
  slug: shopmonkey-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shopmonkey/refs/heads/main/openapi/shopmonkey-openapi.yml
- filename: shopmonkey-openapi.yml
  format: yaml
  label: Shopmonkey Vehicles API
  slug: shopmonkey-vehicles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shopmonkey/refs/heads/main/openapi/shopmonkey-openapi.yml
- filename: shopmonkey-openapi.yml
  format: yaml
  label: Shopmonkey Inventory & Parts API
  slug: shopmonkey-inventory-parts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shopmonkey/refs/heads/main/openapi/shopmonkey-openapi.yml
- filename: shopmonkey-openapi.yml
  format: yaml
  label: Shopmonkey Invoices & Payments API
  slug: shopmonkey-invoices-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shopmonkey/refs/heads/main/openapi/shopmonkey-openapi.yml
- filename: shopmonkey-openapi.yml
  format: yaml
  label: Shopmonkey Appointments API
  slug: shopmonkey-appointments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shopmonkey/refs/heads/main/openapi/shopmonkey-openapi.yml
- filename: shopmonkey-openapi.yml
  format: yaml
  label: Shopmonkey Employees API
  slug: shopmonkey-employees-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shopmonkey/refs/heads/main/openapi/shopmonkey-openapi.yml
- filename: shopmonkey-openapi.yml
  format: yaml
  label: Shopmonkey Locations API
  slug: shopmonkey-locations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shopmonkey/refs/heads/main/openapi/shopmonkey-openapi.yml
- filename: shopmonkey-openapi.yml
  format: yaml
  label: Shopmonkey Webhooks API
  slug: shopmonkey-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shopmonkey/refs/heads/main/openapi/shopmonkey-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  - 0 issuewild "amazon.com"
  - 0 issuewild "letsencrypt.org"
  - 0 issue "amazon.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: shopmonkey.io
  spf: true
- caa:
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: shopmonkey.dev
  spf: true
hosts:
- cert_expires: Sep 23 18:23:51 2026 GMT
  host: www.shopmonkey.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 22 22:15:19 2026 GMT
  host: shopmonkey.dev
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  5 00:36:27 2026 GMT
  host: api.shopmonkey.cloud
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Shopmonkey Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Shopmonkey, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Shopmonkey
provider_slug: shopmonkey
slug: shopmonkey-domain-security
source_filename: shopmonkey-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.shopmonkey.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 18:23:51 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: shopmonkey.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 22 22:15:19 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.shopmonkey.cloud\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 00:36:27 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: shopmonkey.io\n  dnssec: false\n  caa:\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issue \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: shopmonkey.dev\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc:\
  \ true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/shopmonkey/refs/heads/main/security/shopmonkey-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Auto Repair
- Shop Management
- Field Service
- REST
- Not GraphQL
---
