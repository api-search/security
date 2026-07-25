---
api_specs:
- filename: backstage-events-asyncapi.yml
  format: yaml
  label: Backstage Events System
  slug: events-system
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/backstage/refs/heads/main/asyncapi/backstage-events-asyncapi.yml
- filename: backstage-actions-api-openapi.yml
  format: yaml
  label: Backstage Actions API
  slug: backstage-actions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/backstage/refs/heads/main/openapi/backstage-actions-api-openapi.yml
- filename: backstage-authentication-api-openapi.yml
  format: yaml
  label: Backstage Authentication API
  slug: backstage-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/backstage/refs/heads/main/openapi/backstage-authentication-api-openapi.yml
- filename: backstage-authorization-api-openapi.yml
  format: yaml
  label: Backstage Authorization API
  slug: backstage-authorization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/backstage/refs/heads/main/openapi/backstage-authorization-api-openapi.yml
- filename: backstage-documentation-api-openapi.yml
  format: yaml
  label: Backstage Documentation API
  slug: backstage-documentation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/backstage/refs/heads/main/openapi/backstage-documentation-api-openapi.yml
- filename: backstage-entities-api-openapi.yml
  format: yaml
  label: Backstage Entities API
  slug: backstage-entities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/backstage/refs/heads/main/openapi/backstage-entities-api-openapi.yml
- filename: backstage-locations-api-openapi.yml
  format: yaml
  label: Backstage Locations API
  slug: backstage-locations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/backstage/refs/heads/main/openapi/backstage-locations-api-openapi.yml
- filename: backstage-metadata-api-openapi.yml
  format: yaml
  label: Backstage Metadata API
  slug: backstage-metadata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/backstage/refs/heads/main/openapi/backstage-metadata-api-openapi.yml
- filename: backstage-search-api-openapi.yml
  format: yaml
  label: Backstage Search API
  slug: backstage-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/backstage/refs/heads/main/openapi/backstage-search-api-openapi.yml
- filename: backstage-sync-api-openapi.yml
  format: yaml
  label: Backstage Sync API
  slug: backstage-sync-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/backstage/refs/heads/main/openapi/backstage-sync-api-openapi.yml
- filename: backstage-tasks-api-openapi.yml
  format: yaml
  label: Backstage Tasks API
  slug: backstage-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/backstage/refs/heads/main/openapi/backstage-tasks-api-openapi.yml
- filename: backstage-templates-api-openapi.yml
  format: yaml
  label: Backstage Templates API
  slug: backstage-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/backstage/refs/heads/main/openapi/backstage-templates-api-openapi.yml
- filename: backstage-token-verification-api-openapi.yml
  format: yaml
  label: Backstage Token Verification API
  slug: backstage-token-verification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/backstage/refs/heads/main/openapi/backstage-token-verification-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: backstage.io
  spf: true
hosts:
- cert_expires: Sep 27 15:01:52 2026 GMT
  host: backstage.io
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Backstage Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Backstage, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Backstage
provider_slug: backstage
slug: backstage-domain-security
source_filename: backstage-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: backstage.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 27 15:01:52 2026 GMT\n  hsts: false\ndomains:\n- domain: backstage.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/backstage/refs/heads/main/security/backstage-domain-security.yml
summary_line: TLSv1.3
tags:
- Developer Portal
- Internal Developer Platform
- Software Catalog
- Open Source
---
