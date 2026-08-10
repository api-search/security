---
api_specs:
- filename: umbra-client-credentials-api-openapi.yml
  format: yaml
  label: Umbra Client Credentials API
  slug: umbra-client-credentials-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/umbra/refs/heads/main/openapi/umbra-client-credentials-api-openapi.yml
- filename: umbra-collections-api-openapi.yml
  format: yaml
  label: Umbra Collections API
  slug: umbra-collections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/umbra/refs/heads/main/openapi/umbra-collections-api-openapi.yml
- filename: umbra-collectmetadata-api-openapi.yml
  format: yaml
  label: Umbra Collect Metadata API
  slug: umbra-collectmetadata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/umbra/refs/heads/main/openapi/umbra-collectmetadata-api-openapi.yml
- filename: umbra-collects-api-openapi.yml
  format: yaml
  label: Umbra Collects API
  slug: umbra-collects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/umbra/refs/heads/main/openapi/umbra-collects-api-openapi.yml
- filename: umbra-deliveryconfig-api-openapi.yml
  format: yaml
  label: Umbra Delivery Config API
  slug: umbra-deliveryconfig-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/umbra/refs/heads/main/openapi/umbra-deliveryconfig-api-openapi.yml
- filename: umbra-feasibility-api-openapi.yml
  format: yaml
  label: Umbra Feasibility API
  slug: umbra-feasibility-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/umbra/refs/heads/main/openapi/umbra-feasibility-api-openapi.yml
- filename: umbra-organizations-api-openapi.yml
  format: yaml
  label: Umbra Organizations API
  slug: umbra-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/umbra/refs/heads/main/openapi/umbra-organizations-api-openapi.yml
- filename: umbra-preview-api-openapi.yml
  format: yaml
  label: Umbra Preview API
  slug: umbra-preview-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/umbra/refs/heads/main/openapi/umbra-preview-api-openapi.yml
- filename: umbra-preview-image-api-openapi.yml
  format: yaml
  label: Umbra Preview Image API
  slug: umbra-preview-image-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/umbra/refs/heads/main/openapi/umbra-preview-image-api-openapi.yml
- filename: umbra-product-constraints-api-openapi.yml
  format: yaml
  label: Umbra Product Constraints API
  slug: umbra-product-constraints-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/umbra/refs/heads/main/openapi/umbra-product-constraints-api-openapi.yml
- filename: umbra-restricted-access-areas-api-openapi.yml
  format: yaml
  label: Umbra Restricted Access Areas API
  slug: umbra-restricted-access-areas-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/umbra/refs/heads/main/openapi/umbra-restricted-access-areas-api-openapi.yml
- filename: umbra-search-api-openapi.yml
  format: yaml
  label: Umbra Search API
  slug: umbra-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/umbra/refs/heads/main/openapi/umbra-search-api-openapi.yml
- filename: umbra-tasks-api-openapi.yml
  format: yaml
  label: Umbra Tasks API
  slug: umbra-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/umbra/refs/heads/main/openapi/umbra-tasks-api-openapi.yml
- filename: umbra-thumbnail-api-openapi.yml
  format: yaml
  label: Umbra Thumbnail API
  slug: umbra-thumbnail-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/umbra/refs/heads/main/openapi/umbra-thumbnail-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: umbra.space
  spf: true
hosts:
- cert_expires: Oct  7 09:25:20 2026 GMT
  host: umbra.space
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 19 22:58:14 2026 GMT
  host: docs.canopy.umbra.space
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 23 23:59:59 2027 GMT
  host: api.canopy.umbra.space
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Umbra Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Umbra, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Umbra
provider_slug: umbra
slug: umbra-domain-security
source_filename: umbra-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: umbra.space\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 09:25:20 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.canopy.umbra.space\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 19 22:58:14 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.canopy.umbra.space\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 23 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: umbra.space\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/umbra/refs/heads/main/security/umbra-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Satellite Imagery
- Synthetic Aperture Radar
- Earth Observation
- Geospatial
- Space
- STAC
- Remote Sensing
- Tasking
- Defense and Intelligence
- Company
---
