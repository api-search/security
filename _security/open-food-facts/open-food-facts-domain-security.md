---
api_specs:
- filename: open-food-facts-api-v2-openapi.yml
  format: yaml
  label: Open Food Facts API v2
  slug: open-food-facts-api-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/open-food-facts/refs/heads/main/openapi/open-food-facts-api-v2-openapi.yml
- filename: open-food-facts-api-v3-openapi.yml
  format: yaml
  label: Open Food Facts API v3
  slug: open-food-facts-api-v3
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/open-food-facts/refs/heads/main/openapi/open-food-facts-api-v3-openapi.yml
- filename: open-food-facts-open-prices-openapi.yml
  format: yaml
  label: Open Prices API
  slug: open-food-facts-open-prices
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/open-food-facts/refs/heads/main/openapi/open-food-facts-open-prices-openapi.yml
- filename: open-food-facts-search-a-licious-openapi.json
  format: json
  label: Search-a-licious API
  slug: open-food-facts-search-a-licious
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/open-food-facts/refs/heads/main/openapi/open-food-facts-search-a-licious-openapi.json
- filename: open-food-facts-folksonomy-openapi.json
  format: json
  label: Folksonomy Engine API
  slug: open-food-facts-folksonomy
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/open-food-facts/refs/heads/main/openapi/open-food-facts-folksonomy-openapi.json
- filename: open-food-facts-facets-knowledge-panels-openapi.json
  format: json
  label: Facets Knowledge Panels API
  slug: open-food-facts-facets-knowledge-panels
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/open-food-facts/refs/heads/main/openapi/open-food-facts-facets-knowledge-panels-openapi.json
- filename: open-food-facts-nutripatrol-openapi.json
  format: json
  label: NutriPatrol API
  slug: open-food-facts-nutripatrol
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/open-food-facts/refs/heads/main/openapi/open-food-facts-nutripatrol-openapi.json
- filename: open-food-facts-cgi-api-openapi.yml
  format: yaml
  label: Open Food Facts Cgi API
  slug: open-food-facts-cgi-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/open-food-facts/refs/heads/main/openapi/open-food-facts-cgi-api-openapi.yml
- filename: open-food-facts-product-api-openapi.yml
  format: yaml
  label: Open Food Facts Product API
  slug: open-food-facts-product-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/open-food-facts/refs/heads/main/openapi/open-food-facts-product-api-openapi.yml
- filename: open-food-facts-search-api-openapi.yml
  format: yaml
  label: Open Food Facts Search API
  slug: open-food-facts-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/open-food-facts/refs/heads/main/openapi/open-food-facts-search-api-openapi.yml
- filename: open-food-facts-taxonomy-api-openapi.yml
  format: yaml
  label: Open Food Facts Taxonomy API
  slug: open-food-facts-taxonomy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/open-food-facts/refs/heads/main/openapi/open-food-facts-taxonomy-api-openapi.yml
- filename: open-food-facts-taxonomy-suggestions-api-openapi.yml
  format: yaml
  label: Open Food Facts Taxonomy Suggestions API
  slug: open-food-facts-taxonomy-suggestions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/open-food-facts/refs/heads/main/openapi/open-food-facts-taxonomy-suggestions-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: openfoodfacts.org
  spf: true
hosts:
- cert_expires: Nov 19 04:36:26 2026 GMT
  host: world.openfoodfacts.org
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 24 06:52:09 2026 GMT
  host: prices.openfoodfacts.org
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 17 06:54:24 2026 GMT
  host: search.openfoodfacts.org
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Open Food Facts Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Open Food Facts, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Open Food Facts
provider_slug: open-food-facts
slug: open-food-facts-domain-security
source_filename: open-food-facts-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: world.openfoodfacts.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 19 04:36:26 2026 GMT\n  hsts: false\n- host: prices.openfoodfacts.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 24 06:52:09 2026 GMT\n  hsts: false\n- host: search.openfoodfacts.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 17 06:54:24 2026 GMT\n  hsts: null\ndomains:\n- domain: openfoodfacts.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/open-food-facts/refs/heads/main/security/open-food-facts-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Food
- Nutrition
- Open Data
- Product Data
- Barcodes
- Taxonomy
- Prices
- Search
---
