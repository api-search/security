---
api_specs:
- filename: contraforce-agent-tools-api-openapi.yml
  format: yaml
  label: Contraforce Agent Tools API
  slug: contraforce-agent-tools-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/contraforce/refs/heads/main/openapi/contraforce-agent-tools-api-openapi.yml
- filename: contraforce-azure-resources-api-openapi.yml
  format: yaml
  label: Contraforce Azure resources API
  slug: contraforce-azure-resources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/contraforce/refs/heads/main/openapi/contraforce-azure-resources-api-openapi.yml
- filename: contraforce-cross-workspace-data-sources-api-openapi.yml
  format: yaml
  label: Contraforce Cross-workspace data sources API
  slug: contraforce-cross-workspace-data-sources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/contraforce/refs/heads/main/openapi/contraforce-cross-workspace-data-sources-api-openapi.yml
- filename: contraforce-cross-workspace-gamebooks-api-openapi.yml
  format: yaml
  label: Contraforce Cross-workspace gamebooks API
  slug: contraforce-cross-workspace-gamebooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/contraforce/refs/heads/main/openapi/contraforce-cross-workspace-gamebooks-api-openapi.yml
- filename: contraforce-cross-workspace-incidents-api-openapi.yml
  format: yaml
  label: Contraforce Cross-workspace incidents API
  slug: contraforce-cross-workspace-incidents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/contraforce/refs/heads/main/openapi/contraforce-cross-workspace-incidents-api-openapi.yml
- filename: contraforce-data-sources-api-openapi.yml
  format: yaml
  label: Contraforce Data sources API
  slug: contraforce-data-sources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/contraforce/refs/heads/main/openapi/contraforce-data-sources-api-openapi.yml
- filename: contraforce-export-api-openapi.yml
  format: yaml
  label: Contraforce Export API
  slug: contraforce-export-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/contraforce/refs/heads/main/openapi/contraforce-export-api-openapi.yml
- filename: contraforce-gamebooks-api-openapi.yml
  format: yaml
  label: Contraforce Gamebooks API
  slug: contraforce-gamebooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/contraforce/refs/heads/main/openapi/contraforce-gamebooks-api-openapi.yml
- filename: contraforce-incidents-api-openapi.yml
  format: yaml
  label: Contraforce Incidents API
  slug: contraforce-incidents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/contraforce/refs/heads/main/openapi/contraforce-incidents-api-openapi.yml
- filename: contraforce-investigation-api-openapi.yml
  format: yaml
  label: Contraforce Investigation API
  slug: contraforce-investigation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/contraforce/refs/heads/main/openapi/contraforce-investigation-api-openapi.yml
- filename: contraforce-service-accounts-api-openapi.yml
  format: yaml
  label: Contraforce Service accounts API
  slug: contraforce-service-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/contraforce/refs/heads/main/openapi/contraforce-service-accounts-api-openapi.yml
- filename: contraforce-service-tickets-api-openapi.yml
  format: yaml
  label: Contraforce Service tickets API
  slug: contraforce-service-tickets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/contraforce/refs/heads/main/openapi/contraforce-service-tickets-api-openapi.yml
- filename: contraforce-users-api-openapi.yml
  format: yaml
  label: Contraforce Users API
  slug: contraforce-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/contraforce/refs/heads/main/openapi/contraforce-users-api-openapi.yml
- filename: contraforce-webhooks-api-openapi.yml
  format: yaml
  label: Contraforce Webhooks API
  slug: contraforce-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/contraforce/refs/heads/main/openapi/contraforce-webhooks-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: contraforce.com
  spf: true
hosts:
- cert_expires: Nov 12 23:42:43 2026 GMT
  host: www.contraforce.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Contraforce Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Contraforce, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Contraforce
provider_slug: contraforce
slug: contraforce-domain-security
source_filename: contraforce-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-10'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.contraforce.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 12 23:42:43 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: contraforce.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/contraforce/refs/heads/main/security/contraforce-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Security
- SaaS
- Cybersecurity
- Microsoft
- MSP
---
