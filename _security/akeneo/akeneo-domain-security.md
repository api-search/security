---
api_specs:
- filename: akeneo-asset-manager-api-openapi.yml
  format: yaml
  label: Akeneo Asset Manager API
  slug: akeneo-asset-manager-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/akeneo/refs/heads/main/openapi/akeneo-asset-manager-api-openapi.yml
- filename: akeneo-attributes-api-openapi.yml
  format: yaml
  label: Akeneo Attributes API
  slug: akeneo-attributes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/akeneo/refs/heads/main/openapi/akeneo-attributes-api-openapi.yml
- filename: akeneo-authentication-api-openapi.yml
  format: yaml
  label: Akeneo Authentication API
  slug: akeneo-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/akeneo/refs/heads/main/openapi/akeneo-authentication-api-openapi.yml
- filename: akeneo-catalogs-api-openapi.yml
  format: yaml
  label: Akeneo Catalogs API
  slug: akeneo-catalogs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/akeneo/refs/heads/main/openapi/akeneo-catalogs-api-openapi.yml
- filename: akeneo-categories-api-openapi.yml
  format: yaml
  label: Akeneo Categories API
  slug: akeneo-categories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/akeneo/refs/heads/main/openapi/akeneo-categories-api-openapi.yml
- filename: akeneo-channels-api-openapi.yml
  format: yaml
  label: Akeneo Channels API
  slug: akeneo-channels-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/akeneo/refs/heads/main/openapi/akeneo-channels-api-openapi.yml
- filename: akeneo-currencies-api-openapi.yml
  format: yaml
  label: Akeneo Currencies API
  slug: akeneo-currencies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/akeneo/refs/heads/main/openapi/akeneo-currencies-api-openapi.yml
- filename: akeneo-families-api-openapi.yml
  format: yaml
  label: Akeneo Families API
  slug: akeneo-families-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/akeneo/refs/heads/main/openapi/akeneo-families-api-openapi.yml
- filename: akeneo-locales-api-openapi.yml
  format: yaml
  label: Akeneo Locales API
  slug: akeneo-locales-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/akeneo/refs/heads/main/openapi/akeneo-locales-api-openapi.yml
- filename: akeneo-media-files-api-openapi.yml
  format: yaml
  label: Akeneo Media Files API
  slug: akeneo-media-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/akeneo/refs/heads/main/openapi/akeneo-media-files-api-openapi.yml
- filename: akeneo-product-models-api-openapi.yml
  format: yaml
  label: Akeneo Product Models API
  slug: akeneo-product-models-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/akeneo/refs/heads/main/openapi/akeneo-product-models-api-openapi.yml
- filename: akeneo-products-api-openapi.yml
  format: yaml
  label: Akeneo Products API
  slug: akeneo-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/akeneo/refs/heads/main/openapi/akeneo-products-api-openapi.yml
- filename: akeneo-reference-entities-api-openapi.yml
  format: yaml
  label: Akeneo Reference Entities API
  slug: akeneo-reference-entities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/akeneo/refs/heads/main/openapi/akeneo-reference-entities-api-openapi.yml
- filename: akeneo-system-api-openapi.yml
  format: yaml
  label: Akeneo System API
  slug: akeneo-system-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/akeneo/refs/heads/main/openapi/akeneo-system-api-openapi.yml
- filename: akeneo-workflows-api-openapi.yml
  format: yaml
  label: Akeneo Workflows API
  slug: akeneo-workflows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/akeneo/refs/heads/main/openapi/akeneo-workflows-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: akeneo.com
  spf: true
hosts:
- cert_expires: Aug 18 13:59:22 2026 GMT
  host: www.akeneo.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 15 21:34:56 2026 GMT
  host: api.akeneo.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Akeneo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Akeneo, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Akeneo
provider_slug: akeneo
slug: akeneo-domain-security
source_filename: akeneo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.akeneo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 18 13:59:22 2026 GMT\n  hsts: false\n- host: api.akeneo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 21:34:56 2026 GMT\n  hsts: false\ndomains:\n- domain: akeneo.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/akeneo/refs/heads/main/security/akeneo-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Product Information Management
- PIM
- Product Data
- Catalog Management
- Commerce
- Retail
---
