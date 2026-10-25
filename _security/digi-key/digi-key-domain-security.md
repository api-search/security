---
api_specs:
- filename: digi-key-barcoding-api-openapi.yml
  format: yaml
  label: Digi-Key Barcoding API
  slug: digi-key-barcoding-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/digi-key/refs/heads/main/openapi/digi-key-barcoding-api-openapi.yml
- filename: digi-key-bondedinventory-api-openapi.yml
  format: yaml
  label: Digi-Key Bonded Inventory API
  slug: digi-key-bondedinventory-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/digi-key/refs/heads/main/openapi/digi-key-bondedinventory-api-openapi.yml
- filename: digi-key-customerresource-api-openapi.yml
  format: yaml
  label: Digi-Key Customer Resource API
  slug: digi-key-customerresource-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/digi-key/refs/heads/main/openapi/digi-key-customerresource-api-openapi.yml
- filename: digi-key-lists-api-openapi.yml
  format: yaml
  label: Digi-Key Lists API
  slug: digi-key-lists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/digi-key/refs/heads/main/openapi/digi-key-lists-api-openapi.yml
- filename: digi-key-orderhistory-api-openapi.yml
  format: yaml
  label: Digi-Key Order History API
  slug: digi-key-orderhistory-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/digi-key/refs/heads/main/openapi/digi-key-orderhistory-api-openapi.yml
- filename: digi-key-ordermanagement-api-openapi.yml
  format: yaml
  label: Digi-Key Order Management API
  slug: digi-key-ordermanagement-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/digi-key/refs/heads/main/openapi/digi-key-ordermanagement-api-openapi.yml
- filename: digi-key-orders-api-openapi.yml
  format: yaml
  label: Digi-Key Orders API
  slug: digi-key-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/digi-key/refs/heads/main/openapi/digi-key-orders-api-openapi.yml
- filename: digi-key-packlist-api-openapi.yml
  format: yaml
  label: Digi-Key Pack List API
  slug: digi-key-packlist-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/digi-key/refs/heads/main/openapi/digi-key-packlist-api-openapi.yml
- filename: digi-key-parts-api-openapi.yml
  format: yaml
  label: Digi-Key Parts API
  slug: digi-key-parts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/digi-key/refs/heads/main/openapi/digi-key-parts-api-openapi.yml
- filename: digi-key-pcn-api-openapi.yml
  format: yaml
  label: Digi-Key Pcn API
  slug: digi-key-pcn-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/digi-key/refs/heads/main/openapi/digi-key-pcn-api-openapi.yml
- filename: digi-key-quotes-api-openapi.yml
  format: yaml
  label: Digi-Key Quotes API
  slug: digi-key-quotes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/digi-key/refs/heads/main/openapi/digi-key-quotes-api-openapi.yml
- filename: digi-key-product-search-api-openapi.yml
  format: yaml
  label: Digi-Key Product Search API
  slug: digi-key-product-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/digi-key/refs/heads/main/openapi/digi-key-product-search-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: digikey.com
  spf: true
hosts:
- cert_expires: Dec 22 17:17:15 2026 GMT
  host: www.digikey.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Digi Key Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Digi-Key, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Digi-Key
provider_slug: digi-key
slug: digi-key-domain-security
source_filename: digi-key-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.digikey.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 22 17:17:15 2026 GMT\n  hsts: null\ndomains:\n- domain: digikey.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/digi-key/refs/heads/main/security/digi-key-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Shopping
- Public APIs
- Electronic Components
- Distribution
- Ordering
- Product Search
- Pricing
- Inventory
- Supply Chain
---
