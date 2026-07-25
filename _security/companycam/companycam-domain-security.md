---
api_specs:
- filename: companycam-checklists-api-openapi.yml
  format: yaml
  label: CompanyCam Checklists API
  slug: companycam-checklists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/companycam/refs/heads/main/openapi/companycam-checklists-api-openapi.yml
- filename: companycam-company-api-openapi.yml
  format: yaml
  label: CompanyCam Company API
  slug: companycam-company-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/companycam/refs/heads/main/openapi/companycam-company-api-openapi.yml
- filename: companycam-groups-api-openapi.yml
  format: yaml
  label: CompanyCam Groups API
  slug: companycam-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/companycam/refs/heads/main/openapi/companycam-groups-api-openapi.yml
- filename: companycam-photos-api-openapi.yml
  format: yaml
  label: CompanyCam Photos API
  slug: companycam-photos-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/companycam/refs/heads/main/openapi/companycam-photos-api-openapi.yml
- filename: companycam-projects-api-openapi.yml
  format: yaml
  label: CompanyCam Projects API
  slug: companycam-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/companycam/refs/heads/main/openapi/companycam-projects-api-openapi.yml
- filename: companycam-tags-api-openapi.yml
  format: yaml
  label: CompanyCam Tags API
  slug: companycam-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/companycam/refs/heads/main/openapi/companycam-tags-api-openapi.yml
- filename: companycam-templates-api-openapi.yml
  format: yaml
  label: CompanyCam Templates API
  slug: companycam-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/companycam/refs/heads/main/openapi/companycam-templates-api-openapi.yml
- filename: companycam-users-api-openapi.yml
  format: yaml
  label: CompanyCam Users API
  slug: companycam-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/companycam/refs/heads/main/openapi/companycam-users-api-openapi.yml
- filename: companycam-videos-api-openapi.yml
  format: yaml
  label: CompanyCam Videos API
  slug: companycam-videos-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/companycam/refs/heads/main/openapi/companycam-videos-api-openapi.yml
- filename: companycam-webhooks-api-openapi.yml
  format: yaml
  label: CompanyCam Webhooks API
  slug: companycam-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/companycam/refs/heads/main/openapi/companycam-webhooks-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "amazon.com"
  - 0 issue "digicert.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: companycam.com
  spf: true
hosts:
- cert_expires: Nov 27 23:59:59 2026 GMT
  host: companycam.com
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  5 23:59:59 2026 GMT
  host: api.companycam.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Companycam Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CompanyCam, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: CompanyCam
provider_slug: companycam
slug: companycam-domain-security
source_filename: companycam-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: companycam.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 27 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\n- host: api.companycam.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: companycam.com\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"digicert.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/companycam/refs/heads/main/security/companycam-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Construction
- Photos
- Field Service
- Project Management
- Contractors
- Documentation
- Webhooks
---
