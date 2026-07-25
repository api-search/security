---
api_specs:
- filename: fivetran-connections-api-openapi.yml
  format: yaml
  label: Fivetran Connections API
  slug: fivetran-connections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fivetran/refs/heads/main/openapi/fivetran-connections-api-openapi.yml
- filename: fivetran-destinations-api-openapi.yml
  format: yaml
  label: Fivetran Destinations API
  slug: fivetran-destinations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fivetran/refs/heads/main/openapi/fivetran-destinations-api-openapi.yml
- filename: fivetran-groups-api-openapi.yml
  format: yaml
  label: Fivetran Groups API
  slug: fivetran-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fivetran/refs/heads/main/openapi/fivetran-groups-api-openapi.yml
- filename: fivetran-metadata-api-openapi.yml
  format: yaml
  label: Fivetran Metadata API
  slug: fivetran-metadata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fivetran/refs/heads/main/openapi/fivetran-metadata-api-openapi.yml
- filename: fivetran-roles-api-openapi.yml
  format: yaml
  label: Fivetran Roles API
  slug: fivetran-roles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fivetran/refs/heads/main/openapi/fivetran-roles-api-openapi.yml
- filename: fivetran-teams-api-openapi.yml
  format: yaml
  label: Fivetran Teams API
  slug: fivetran-teams-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fivetran/refs/heads/main/openapi/fivetran-teams-api-openapi.yml
- filename: fivetran-users-api-openapi.yml
  format: yaml
  label: Fivetran Users API
  slug: fivetran-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fivetran/refs/heads/main/openapi/fivetran-users-api-openapi.yml
- filename: fivetran-webhooks-api-openapi.yml
  format: yaml
  label: Fivetran Webhooks API
  slug: fivetran-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fivetran/refs/heads/main/openapi/fivetran-webhooks-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: fivetran.com
  spf: true
hosts:
- cert_expires: Sep 28 11:46:42 2026 GMT
  host: www.fivetran.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 19 20:21:54 2026 GMT
  host: fivetran.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 19 19:04:09 2026 GMT
  host: api.fivetran.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Fivetran Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Fivetran, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Fivetran
provider_slug: fivetran
slug: fivetran-domain-security
source_filename: fivetran-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.fivetran.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 11:46:42 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: fivetran.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 19 20:21:54 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.fivetran.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 19 19:04:09 2026 GMT\n  hsts: null\ndomains:\n- domain: fivetran.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fivetran/refs/heads/main/security/fivetran-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Connectors
- Data Integration
- Data Pipeline
- ETL
- SaaS
- Unified API
---
