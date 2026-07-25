---
api_specs:
- filename: ostrom-auth-api-openapi.yml
  format: yaml
  label: Ostrom Auth API
  slug: ostrom-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ostrom/refs/heads/main/openapi/ostrom-auth-api-openapi.yml
- filename: ostrom-contracts-api-openapi.yml
  format: yaml
  label: Ostrom Contracts API
  slug: ostrom-contracts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ostrom/refs/heads/main/openapi/ostrom-contracts-api-openapi.yml
- filename: ostrom-orders-api-openapi.yml
  format: yaml
  label: Ostrom Orders API
  slug: ostrom-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ostrom/refs/heads/main/openapi/ostrom-orders-api-openapi.yml
- filename: ostrom-prices-api-openapi.yml
  format: yaml
  label: Ostrom Prices API
  slug: ostrom-prices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ostrom/refs/heads/main/openapi/ostrom-prices-api-openapi.yml
- filename: ostrom-products-api-openapi.yml
  format: yaml
  label: Ostrom Products API
  slug: ostrom-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ostrom/refs/heads/main/openapi/ostrom-products-api-openapi.yml
- filename: ostrom-users-api-openapi.yml
  format: yaml
  label: Ostrom Users API
  slug: ostrom-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ostrom/refs/heads/main/openapi/ostrom-users-api-openapi.yml
- filename: ostrom-webhooks-api-openapi.yml
  format: yaml
  label: Ostrom Webhooks API
  slug: ostrom-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ostrom/refs/heads/main/openapi/ostrom-webhooks-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: ostrom.de
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: ostrom-api.io
  spf: false
hosts:
- cert_expires: Oct 15 10:16:22 2026 GMT
  host: ostrom.de
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  1 23:59:59 2026 GMT
  host: sandbox.ostrom-api.io
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.2
- cert_expires: Oct  1 23:59:59 2026 GMT
  host: production.ostrom-api.io
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Ostrom Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ostrom, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Ostrom
provider_slug: ostrom
slug: ostrom-domain-security
source_filename: ostrom-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ostrom.de\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 15 10:16:22 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: sandbox.ostrom-api.io\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct  1 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: production.ostrom-api.io\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct  1 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: ostrom.de\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: ostrom-api.io\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ostrom/refs/heads/main/security/ostrom-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Energy
- Electricity
- Green Energy
- Smart Meter
- Dynamic Pricing
- Germany
- Sustainability
- Webhooks
- API
---
