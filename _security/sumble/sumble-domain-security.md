---
api_specs:
- filename: sumble-contact-lists-api-openapi.yml
  format: yaml
  label: Sumble contact-lists API
  slug: sumble-contact-lists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sumble/refs/heads/main/openapi/sumble-contact-lists-api-openapi.yml
- filename: sumble-jobs-api-openapi.yml
  format: yaml
  label: Sumble jobs API
  slug: sumble-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sumble/refs/heads/main/openapi/sumble-jobs-api-openapi.yml
- filename: sumble-organization-lists-api-openapi.yml
  format: yaml
  label: Sumble organization-lists API
  slug: sumble-organization-lists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sumble/refs/heads/main/openapi/sumble-organization-lists-api-openapi.yml
- filename: sumble-organizations-api-openapi.yml
  format: yaml
  label: Sumble organizations API
  slug: sumble-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sumble/refs/heads/main/openapi/sumble-organizations-api-openapi.yml
- filename: sumble-people-api-openapi.yml
  format: yaml
  label: Sumble people API
  slug: sumble-people-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sumble/refs/heads/main/openapi/sumble-people-api-openapi.yml
- filename: sumble-projects-api-openapi.yml
  format: yaml
  label: Sumble projects API
  slug: sumble-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sumble/refs/heads/main/openapi/sumble-projects-api-openapi.yml
- filename: sumble-signals-api-openapi.yml
  format: yaml
  label: Sumble signals API
  slug: sumble-signals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sumble/refs/heads/main/openapi/sumble-signals-api-openapi.yml
- filename: sumble-support-api-openapi.yml
  format: yaml
  label: Sumble support API
  slug: sumble-support-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sumble/refs/heads/main/openapi/sumble-support-api-openapi.yml
- filename: sumble-teams-api-openapi.yml
  format: yaml
  label: Sumble teams API
  slug: sumble-teams-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sumble/refs/heads/main/openapi/sumble-teams-api-openapi.yml
- filename: sumble-technologies-api-openapi.yml
  format: yaml
  label: Sumble technologies API
  slug: sumble-technologies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sumble/refs/heads/main/openapi/sumble-technologies-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: sumble.com
  spf: true
hosts:
- cert_expires: Nov 11 04:44:09 2026 GMT
  host: sumble.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  7 03:25:51 2026 GMT
  host: docs.sumble.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 22 03:24:16 2026 GMT
  host: api.sumble.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Sumble Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Sumble, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Sumble
provider_slug: sumble
slug: sumble-domain-security
source_filename: sumble-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: sumble.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 11 04:44:09 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.sumble.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 03:25:51 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.sumble.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 22 03:24:16 2026 GMT\n  hsts: null\ndomains:\n- domain: sumble.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sumble/refs/heads/main/security/sumble-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Account Intelligence
- Sales Intelligence
- Data Enrichment
- Go-To-Market
- Technographics
- People Data
- Job Posts
- Signals
- MCP
---
