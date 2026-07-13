---
api_specs:
- filename: takealot-seller-openapi.yml
  format: yaml
  label: Takealot Seller API
  slug: seller-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/takealot/refs/heads/main/openapi/takealot-seller-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: takealot.com
  spf: true
hosts:
- cert_expires: Dec  4 12:13:26 2026 GMT
  host: www.takealot.com
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  4 12:13:26 2026 GMT
  host: seller-api.takealot.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Takealot Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Takealot, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Takealot
provider_slug: takealot
slug: takealot-domain-security
source_filename: takealot-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.takealot.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  4 12:13:26 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\n- host: seller-api.takealot.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  4 12:13:26 2026 GMT\n  hsts: null\ndomains:\n- domain: takealot.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/takealot/refs/heads/main/security/takealot-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Commerce
- E-Commerce
- Marketplace
- Retail
- Marketplace Sellers
- Offers
- Orders
- Sales
- Stock Management
- Fulfilment
- Logistics
- Food Delivery
- South Africa
- Africa
- Naspers
- Prosus
---
