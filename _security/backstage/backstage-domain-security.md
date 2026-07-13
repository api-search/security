---
api_specs:
- filename: backstage-catalog-openapi.yml
  format: yaml
  label: Backstage Catalog API
  slug: catalog-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/backstage/refs/heads/main/openapi/backstage-catalog-openapi.yml
- filename: backstage-scaffolder-openapi.yml
  format: yaml
  label: Backstage Scaffolder API
  slug: scaffolder-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/backstage/refs/heads/main/openapi/backstage-scaffolder-openapi.yml
- filename: backstage-auth-openapi.yml
  format: yaml
  label: Backstage Auth API
  slug: auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/backstage/refs/heads/main/openapi/backstage-auth-openapi.yml
- filename: backstage-techdocs-openapi.yml
  format: yaml
  label: Backstage TechDocs API
  slug: techdocs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/backstage/refs/heads/main/openapi/backstage-techdocs-openapi.yml
- filename: backstage-search-openapi.yml
  format: yaml
  label: Backstage Search API
  slug: search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/backstage/refs/heads/main/openapi/backstage-search-openapi.yml
- filename: backstage-permissions-openapi.yml
  format: yaml
  label: Backstage Permissions API
  slug: permissions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/backstage/refs/heads/main/openapi/backstage-permissions-openapi.yml
- filename: backstage-events-asyncapi.yml
  format: yaml
  label: Backstage Events System
  slug: events-system
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/backstage/refs/heads/main/asyncapi/backstage-events-asyncapi.yml
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
