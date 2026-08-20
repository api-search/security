---
api_specs:
- filename: urban-outfitters-creatives-api-openapi.yml
  format: yaml
  label: Urban Outfitters Creatives API
  slug: urban-outfitters-creatives-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/urban-outfitters/refs/heads/main/openapi/urban-outfitters-creatives-api-openapi.yml
- filename: urban-outfitters-inventory-api-openapi.yml
  format: yaml
  label: Urban Outfitters Inventory API
  slug: urban-outfitters-inventory-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/urban-outfitters/refs/heads/main/openapi/urban-outfitters-inventory-api-openapi.yml
- filename: urban-outfitters-links-api-openapi.yml
  format: yaml
  label: Urban Outfitters Links API
  slug: urban-outfitters-links-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/urban-outfitters/refs/heads/main/openapi/urban-outfitters-links-api-openapi.yml
- filename: urban-outfitters-orders-api-openapi.yml
  format: yaml
  label: Urban Outfitters Orders API
  slug: urban-outfitters-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/urban-outfitters/refs/heads/main/openapi/urban-outfitters-orders-api-openapi.yml
- filename: urban-outfitters-products-api-openapi.yml
  format: yaml
  label: Urban Outfitters Products API
  slug: urban-outfitters-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/urban-outfitters/refs/heads/main/openapi/urban-outfitters-products-api-openapi.yml
- filename: urban-outfitters-reports-api-openapi.yml
  format: yaml
  label: Urban Outfitters Reports API
  slug: urban-outfitters-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/urban-outfitters/refs/heads/main/openapi/urban-outfitters-reports-api-openapi.yml
- filename: urban-outfitters-shipments-api-openapi.yml
  format: yaml
  label: Urban Outfitters Shipments API
  slug: urban-outfitters-shipments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/urban-outfitters/refs/heads/main/openapi/urban-outfitters-shipments-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: urban-outfitters.com
  spf: false
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: urbanoutfitters.com
  spf: true
hosts:
- host: www.urban-outfitters.com
  https: false
- cert_expires: Oct 12 23:59:59 2026 GMT
  host: www.urbanoutfitters.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- host: api.rakutenadvertising.com
  https: false
kind: domain-security
layout: security
method: probed
name: Urban Outfitters Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Urban Outfitters, probed live across 3 host(s) and 2 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Urban Outfitters
provider_slug: urban-outfitters
slug: urban-outfitters-domain-security
source_filename: urban-outfitters-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.urban-outfitters.com\n  https: false\n- host: www.urbanoutfitters.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 12 23:59:59 2026 GMT\n  hsts: null\n- host: api.rakutenadvertising.com\n  https: false\ndomains:\n- domain: urban-outfitters.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n- domain: urbanoutfitters.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/urban-outfitters/refs/heads/main/security/urban-outfitters-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Retail
- Fashion
- Apparel
- E-Commerce
- Affiliates
- Marketplace
- Fortune 1000
---
