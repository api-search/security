---
api_specs:
- filename: rhythms-access-requests-api-openapi.yml
  format: yaml
  label: Rhythms access_requests API
  slug: rhythms-access-requests-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rhythms/refs/heads/main/openapi/rhythms-access-requests-api-openapi.yml
- filename: rhythms-chat-refresh-threads-api-openapi.yml
  format: yaml
  label: Rhythms chat_refresh_threads API
  slug: rhythms-chat-refresh-threads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rhythms/refs/heads/main/openapi/rhythms-chat-refresh-threads-api-openapi.yml
- filename: rhythms-connector-requests-api-openapi.yml
  format: yaml
  label: Rhythms connector_requests API
  slug: rhythms-connector-requests-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rhythms/refs/heads/main/openapi/rhythms-connector-requests-api-openapi.yml
- filename: rhythms-data-sources-api-openapi.yml
  format: yaml
  label: Rhythms data_sources API
  slug: rhythms-data-sources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rhythms/refs/heads/main/openapi/rhythms-data-sources-api-openapi.yml
- filename: rhythms-documents-api-openapi.yml
  format: yaml
  label: Rhythms documents API
  slug: rhythms-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rhythms/refs/heads/main/openapi/rhythms-documents-api-openapi.yml
- filename: rhythms-explorer-views-api-openapi.yml
  format: yaml
  label: Rhythms explorer_views API
  slug: rhythms-explorer-views-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rhythms/refs/heads/main/openapi/rhythms-explorer-views-api-openapi.yml
- filename: rhythms-labels-api-openapi.yml
  format: yaml
  label: Rhythms labels API
  slug: rhythms-labels-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rhythms/refs/heads/main/openapi/rhythms-labels-api-openapi.yml
- filename: rhythms-mention-access-checks-api-openapi.yml
  format: yaml
  label: Rhythms mention_access_checks API
  slug: rhythms-mention-access-checks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rhythms/refs/heads/main/openapi/rhythms-mention-access-checks-api-openapi.yml
- filename: rhythms-notifications-api-openapi.yml
  format: yaml
  label: Rhythms notifications API
  slug: rhythms-notifications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rhythms/refs/heads/main/openapi/rhythms-notifications-api-openapi.yml
- filename: rhythms-objectives-api-openapi.yml
  format: yaml
  label: Rhythms objectives API
  slug: rhythms-objectives-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rhythms/refs/heads/main/openapi/rhythms-objectives-api-openapi.yml
- filename: rhythms-teams-api-openapi.yml
  format: yaml
  label: Rhythms teams API
  slug: rhythms-teams-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rhythms/refs/heads/main/openapi/rhythms-teams-api-openapi.yml
- filename: rhythms-time-periods-api-openapi.yml
  format: yaml
  label: Rhythms time_periods API
  slug: rhythms-time-periods-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rhythms/refs/heads/main/openapi/rhythms-time-periods-api-openapi.yml
- filename: rhythms-users-api-openapi.yml
  format: yaml
  label: Rhythms users API
  slug: rhythms-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rhythms/refs/heads/main/openapi/rhythms-users-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: rhythms.ai
  spf: true
hosts:
- cert_expires: Sep 20 05:16:10 2026 GMT
  host: www.rhythms.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 10 23:59:59 2026 GMT
  host: api.rhythms.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Rhythms Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Rhythms, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Rhythms
provider_slug: rhythms
slug: rhythms-domain-security
source_filename: rhythms-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.rhythms.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 05:16:10 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.rhythms.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 10 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: rhythms.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rhythms/refs/heads/main/security/rhythms-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Ai
- Productivity
- Goal Tracking
- OKR
- Workflow Automation
- Team Collaboration
- Business Reviews
- MCP
---
