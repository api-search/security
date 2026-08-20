---
api_specs:
- filename: demandbase-b2b-openapi.yml
  format: yaml
  label: Demandbase B2B API
  slug: demandbase-b2b-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/demandbase/refs/heads/main/openapi/demandbase-b2b-openapi.yml
- filename: demandbase-data-export-openapi.yml
  format: yaml
  label: Demandbase Data Export API
  slug: demandbase-data-export-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/demandbase/refs/heads/main/openapi/demandbase-data-export-openapi.yml
- filename: demandbase-data-import-openapi.yml
  format: yaml
  label: Demandbase Data Import API
  slug: demandbase-data-import-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/demandbase/refs/heads/main/openapi/demandbase-data-import-openapi.yml
- filename: demandbase-intent-openapi.yml
  format: yaml
  label: Demandbase Intent API
  slug: demandbase-intent-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/demandbase/refs/heads/main/openapi/demandbase-intent-openapi.yml
- filename: demandbase-admin-openapi.yml
  format: yaml
  label: Demandbase Admin API
  slug: demandbase-admin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/demandbase/refs/heads/main/openapi/demandbase-admin-openapi.yml
- filename: demandbase-usage-openapi.yml
  format: yaml
  label: Demandbase Usage API
  slug: demandbase-usage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/demandbase/refs/heads/main/openapi/demandbase-usage-openapi.yml
- filename: demandbase-custom-sources-openapi.yml
  format: yaml
  label: Demandbase Custom Sources API
  slug: demandbase-custom-sources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/demandbase/refs/heads/main/openapi/demandbase-custom-sources-openapi.yml
- filename: demandbase-auth-openapi.yml
  format: yaml
  label: Demandbase Auth API
  slug: demandbase-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/demandbase/refs/heads/main/openapi/demandbase-auth-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: demandbase.com
  spf: true
hosts:
- cert_expires: Sep 28 20:40:15 2026 GMT
  host: developer.demandbase.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  6 23:23:40 2026 GMT
  host: www.demandbase.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb  8 23:59:59 2027 GMT
  host: api.demandbase.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Demandbase Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Demandbase, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Demandbase
provider_slug: demandbase
slug: demandbase-domain-security
source_filename: demandbase-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developer.demandbase.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 20:40:15 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: www.demandbase.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  6 23:23:40 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.demandbase.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  8 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: demandbase.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/demandbase/refs/heads/main/security/demandbase-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Account Based Marketing
- Advertising
- AI Agents
- B2B Marketing
- Company Data
- Contact Data
- Data Enrichment
- Intent Data
- MCP
- Personalization
- Sales Intelligence
- Technographics
---
