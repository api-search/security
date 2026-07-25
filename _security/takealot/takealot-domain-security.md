---
api_specs:
- filename: takealot-create-a-batch-api-openapi.yml
  format: yaml
  label: Takealot Create a batch API
  slug: takealot-create-a-batch-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/takealot/refs/heads/main/openapi/takealot-create-a-batch-api-openapi.yml
- filename: takealot-create-an-offer-api-openapi.yml
  format: yaml
  label: Takealot Create an offer API
  slug: takealot-create-an-offer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/takealot/refs/heads/main/openapi/takealot-create-an-offer-api-openapi.yml
- filename: takealot-get-a-batch-api-openapi.yml
  format: yaml
  label: Takealot Get a batch API
  slug: takealot-get-a-batch-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/takealot/refs/heads/main/openapi/takealot-get-a-batch-api-openapi.yml
- filename: takealot-get-an-offer-api-openapi.yml
  format: yaml
  label: Takealot Get an offer API
  slug: takealot-get-an-offer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/takealot/refs/heads/main/openapi/takealot-get-an-offer-api-openapi.yml
- filename: takealot-get-offers-api-openapi.yml
  format: yaml
  label: Takealot Get offers API
  slug: takealot-get-offers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/takealot/refs/heads/main/openapi/takealot-get-offers-api-openapi.yml
- filename: takealot-get-offers-count-api-openapi.yml
  format: yaml
  label: Takealot Get offers count API
  slug: takealot-get-offers-count-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/takealot/refs/heads/main/openapi/takealot-get-offers-count-api-openapi.yml
- filename: takealot-get-stock-counts-api-openapi.yml
  format: yaml
  label: Takealot Get stock counts API
  slug: takealot-get-stock-counts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/takealot/refs/heads/main/openapi/takealot-get-stock-counts-api-openapi.yml
- filename: takealot-get-stock-health-api-openapi.yml
  format: yaml
  label: Takealot Get stock health API
  slug: takealot-get-stock-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/takealot/refs/heads/main/openapi/takealot-get-stock-health-api-openapi.yml
- filename: takealot-sales-summary-api-openapi.yml
  format: yaml
  label: Takealot sales summary API
  slug: takealot-sales-summary-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/takealot/refs/heads/main/openapi/takealot-sales-summary-api-openapi.yml
- filename: takealot-update-an-offer-api-openapi.yml
  format: yaml
  label: Takealot Update an offer API
  slug: takealot-update-an-offer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/takealot/refs/heads/main/openapi/takealot-update-an-offer-api-openapi.yml
- filename: takealot-view-sales-api-openapi.yml
  format: yaml
  label: Takealot view sales API
  slug: takealot-view-sales-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/takealot/refs/heads/main/openapi/takealot-view-sales-api-openapi.yml
- filename: takealot-view-sales-orders-api-openapi.yml
  format: yaml
  label: Takealot view sales orders API
  slug: takealot-view-sales-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/takealot/refs/heads/main/openapi/takealot-view-sales-orders-api-openapi.yml
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
