---
api_specs:
- filename: madeiramadeira-callbacks-api-openapi.yml
  format: yaml
  label: Madeiramadeira Callbacks API
  slug: madeiramadeira-callbacks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/madeiramadeira/refs/heads/main/openapi/madeiramadeira-callbacks-api-openapi.yml
- filename: madeiramadeira-categorias-api-openapi.yml
  format: yaml
  label: Madeiramadeira Categorias API
  slug: madeiramadeira-categorias-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/madeiramadeira/refs/heads/main/openapi/madeiramadeira-categorias-api-openapi.yml
- filename: madeiramadeira-financeiro-api-openapi.yml
  format: yaml
  label: Madeiramadeira Financeiro API
  slug: madeiramadeira-financeiro-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/madeiramadeira/refs/heads/main/openapi/madeiramadeira-financeiro-api-openapi.yml
- filename: madeiramadeira-frete-api-openapi.yml
  format: yaml
  label: Madeiramadeira Frete API
  slug: madeiramadeira-frete-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/madeiramadeira/refs/heads/main/openapi/madeiramadeira-frete-api-openapi.yml
- filename: madeiramadeira-mensageria-api-openapi.yml
  format: yaml
  label: Madeiramadeira Mensageria API
  slug: madeiramadeira-mensageria-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/madeiramadeira/refs/heads/main/openapi/madeiramadeira-mensageria-api-openapi.yml
- filename: madeiramadeira-pedido-api-openapi.yml
  format: yaml
  label: Madeiramadeira Pedido API
  slug: madeiramadeira-pedido-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/madeiramadeira/refs/heads/main/openapi/madeiramadeira-pedido-api-openapi.yml
- filename: madeiramadeira-produtos-api-openapi.yml
  format: yaml
  label: Madeiramadeira Produtos API
  slug: madeiramadeira-produtos-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/madeiramadeira/refs/heads/main/openapi/madeiramadeira-produtos-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "sectigo.com"
  - 0 issue "amazon.com"
  - 0 issue "amazonaws.com"
  - 0 issue "amazontrust.com"
  - 0 issue "awstrust.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: madeiramadeira.com.br
  spf: true
- caa:
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "amazon.com"
  - 0 issuewild "digicert.com"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 iodef "mailto:security@postman.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: getpostman.com
  spf: true
hosts:
- cert_expires: Feb 13 20:09:36 2027 GMT
  host: www.madeiramadeira.com.br
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 14 04:19:13 2026 GMT
  host: documenter.getpostman.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 19 23:59:59 2027 GMT
  host: marketplace.madeiramadeira.com.br
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Madeiramadeira Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Madeiramadeira, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Madeiramadeira
provider_slug: madeiramadeira
slug: madeiramadeira-domain-security
source_filename: madeiramadeira-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.madeiramadeira.com.br\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 13 20:09:36 2027 GMT\n  hsts: false\n- host: documenter.getpostman.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 14 04:19:13 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: marketplace.madeiramadeira.com.br\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan 19 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: madeiramadeira.com.br\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"awstrust.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: getpostman.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild\
  \ \"digicert.com\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 iodef \"mailto:security@postman.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/madeiramadeira/refs/heads/main/security/madeiramadeira-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- E-Commerce
- Marketplace
- Retail
- Home Goods
- Furniture
- Brazil
- Seller Integration
- Product Catalog
- Order
- Shipping
- Logistics
---
