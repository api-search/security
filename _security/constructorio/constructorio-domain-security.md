---
api_specs:
- filename: constructorio-search-openapi.yml
  format: yaml
  label: Constructor Search API
  slug: constructor-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/constructorio/refs/heads/main/openapi/constructorio-search-openapi.yml
- filename: constructorio-autocomplete-openapi.yml
  format: yaml
  label: Constructor Autocomplete API
  slug: constructor-autocomplete-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/constructorio/refs/heads/main/openapi/constructorio-autocomplete-openapi.yml
- filename: constructorio-browse-openapi.yml
  format: yaml
  label: Constructor Browse API
  slug: constructor-browse-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/constructorio/refs/heads/main/openapi/constructorio-browse-openapi.yml
- filename: constructorio-recommendations-openapi.yml
  format: yaml
  label: Constructor Recommendations API
  slug: constructor-recommendations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/constructorio/refs/heads/main/openapi/constructorio-recommendations-openapi.yml
- filename: constructorio-image-search-openapi.yml
  format: yaml
  label: Constructor Image Search API
  slug: constructor-image-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/constructorio/refs/heads/main/openapi/constructorio-image-search-openapi.yml
- filename: constructorio-ai-shopping-agent-openapi.yml
  format: yaml
  label: Constructor AI Shopping Agent API
  slug: constructor-ai-shopping-agent-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/constructorio/refs/heads/main/openapi/constructorio-ai-shopping-agent-openapi.yml
- filename: constructorio-catalog-management-openapi.yml
  format: yaml
  label: Constructor Catalog Management API
  slug: constructor-catalog-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/constructorio/refs/heads/main/openapi/constructorio-catalog-management-openapi.yml
- filename: constructorio-catalog-batching-openapi.yml
  format: yaml
  label: Constructor Catalog Batching API
  slug: constructor-catalog-batching-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/constructorio/refs/heads/main/openapi/constructorio-catalog-batching-openapi.yml
- filename: constructorio-configuration-openapi.yml
  format: yaml
  label: Constructor Configuration API
  slug: constructor-configuration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/constructorio/refs/heads/main/openapi/constructorio-configuration-openapi.yml
- filename: constructorio-searchandising-openapi.yml
  format: yaml
  label: Constructor Searchandising API
  slug: constructor-searchandising-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/constructorio/refs/heads/main/openapi/constructorio-searchandising-openapi.yml
- filename: constructorio-quizzes-openapi.yml
  format: yaml
  label: Constructor Quizzes API
  slug: constructor-quizzes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/constructorio/refs/heads/main/openapi/constructorio-quizzes-openapi.yml
- filename: constructorio-offsite-discovery-recommendations-openapi.yml
  format: yaml
  label: Constructor Offsite Discovery Recommendations API
  slug: constructor-offsite-discovery-recommendations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/constructorio/refs/heads/main/openapi/constructorio-offsite-discovery-recommendations-openapi.yml
- filename: constructorio-retail-media-openapi.yml
  format: yaml
  label: Constructor Retail Media API
  slug: constructor-retail-media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/constructorio/refs/heads/main/openapi/constructorio-retail-media-openapi.yml
- filename: constructorio-retail-media-display-ads-openapi.yml
  format: yaml
  label: Constructor Retail Media Display Ads API
  slug: constructor-retail-media-display-ads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/constructorio/refs/heads/main/openapi/constructorio-retail-media-display-ads-openapi.yml
- filename: constructorio-product-details-openapi.yml
  format: yaml
  label: Constructor Product Details API
  slug: constructor-product-details-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/constructorio/refs/heads/main/openapi/constructorio-product-details-openapi.yml
- filename: constructorio-behavioral-actions-openapi.yml
  format: yaml
  label: Constructor Behavioral Actions API
  slug: constructor-behavioral-actions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/constructorio/refs/heads/main/openapi/constructorio-behavioral-actions-openapi.yml
- filename: constructorio-user-profile-openapi.yml
  format: yaml
  label: Constructor User Profile API
  slug: constructor-user-profile-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/constructorio/refs/heads/main/openapi/constructorio-user-profile-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: constructor.com
  spf: true
- caa: []
  dmarc: false
  dnssec: true
  domain: cnstrc.com
  spf: false
hosts:
- cert_expires: Sep 18 08:47:56 2026 GMT
  host: constructor.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 27 05:00:27 2026 GMT
  host: docs.constructor.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb  3 23:59:59 2027 GMT
  host: ac.cnstrc.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Constructorio Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Constructor.io, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Constructor.io
provider_slug: constructorio
slug: constructorio-domain-security
source_filename: constructorio-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-01'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: constructor.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 08:47:56 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.constructor.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 27 05:00:27 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: ac.cnstrc.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  3 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: constructor.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: cnstrc.com\n  dnssec: true\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/constructorio/refs/heads/main/security/constructorio-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Search
- E-Commerce
- Product Discovery
- Recommendations
- Personalization
- Retail
- Retail Media
- Artificial Intelligence
- Merchandising
- Catalog Management
- Agentic Commerce
---
