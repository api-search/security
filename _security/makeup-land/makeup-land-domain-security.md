---
api_specs:
- filename: makeup-land-brands-api-openapi.yml
  format: yaml
  label: makeup.land Brands API
  slug: makeup-land-brands-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/makeup-land/refs/heads/main/openapi/makeup-land-brands-api-openapi.yml
- filename: makeup-land-cart-api-openapi.yml
  format: yaml
  label: makeup.land Cart API
  slug: makeup-land-cart-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/makeup-land/refs/heads/main/openapi/makeup-land-cart-api-openapi.yml
- filename: makeup-land-customers-api-openapi.yml
  format: yaml
  label: makeup.land Customers API
  slug: makeup-land-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/makeup-land/refs/heads/main/openapi/makeup-land-customers-api-openapi.yml
- filename: makeup-land-gift-cards-api-openapi.yml
  format: yaml
  label: makeup.land Gift Cards API
  slug: makeup-land-gift-cards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/makeup-land/refs/heads/main/openapi/makeup-land-gift-cards-api-openapi.yml
- filename: makeup-land-orders-api-openapi.yml
  format: yaml
  label: makeup.land Orders API
  slug: makeup-land-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/makeup-land/refs/heads/main/openapi/makeup-land-orders-api-openapi.yml
- filename: makeup-land-payment-links-api-openapi.yml
  format: yaml
  label: makeup.land Payment Links API
  slug: makeup-land-payment-links-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/makeup-land/refs/heads/main/openapi/makeup-land-payment-links-api-openapi.yml
- filename: makeup-land-products-api-openapi.yml
  format: yaml
  label: makeup.land Products API
  slug: makeup-land-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/makeup-land/refs/heads/main/openapi/makeup-land-products-api-openapi.yml
- filename: makeup-land-proposals-api-openapi.yml
  format: yaml
  label: makeup.land Proposals API
  slug: makeup-land-proposals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/makeup-land/refs/heads/main/openapi/makeup-land-proposals-api-openapi.yml
- filename: makeup-land-register-api-openapi.yml
  format: yaml
  label: makeup.land Register API
  slug: makeup-land-register-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/makeup-land/refs/heads/main/openapi/makeup-land-register-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: makeup.land
  spf: true
hosts:
- cert_expires: Dec  3 07:52:01 2026 GMT
  host: makeup.land
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Makeup Land Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for makeup.land, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: makeup.land
provider_slug: makeup-land
slug: makeup-land-domain-security
source_filename: makeup-land-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: makeup.land\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  3 07:52:01 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: makeup.land\n  dnssec: true\n  caa:\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/makeup-land/refs/heads/main/security/makeup-land-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Cosmetics
- Beauty
- Retail
- E-Commerce
- Shopping
- Loyalty
- Gift Cards
- Product Search
- Agentic Commerce
- MCP
- Agent-Native
- Israel
- A2A
---
