---
api_specs:
- filename: fieldguide-api-api-openapi.yml
  format: yaml
  label: Fieldguide api API
  slug: fieldguide-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fieldguide/refs/heads/main/openapi/fieldguide-api-api-openapi.yml
- filename: fieldguide-comments-api-openapi.yml
  format: yaml
  label: Fieldguide comments API
  slug: fieldguide-comments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fieldguide/refs/heads/main/openapi/fieldguide-comments-api-openapi.yml
- filename: fieldguide-companies-api-openapi.yml
  format: yaml
  label: Fieldguide companies API
  slug: fieldguide-companies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fieldguide/refs/heads/main/openapi/fieldguide-companies-api-openapi.yml
- filename: fieldguide-controls-api-openapi.yml
  format: yaml
  label: Fieldguide controls API
  slug: fieldguide-controls-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fieldguide/refs/heads/main/openapi/fieldguide-controls-api-openapi.yml
- filename: fieldguide-engagements-api-openapi.yml
  format: yaml
  label: Fieldguide engagements API
  slug: fieldguide-engagements-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fieldguide/refs/heads/main/openapi/fieldguide-engagements-api-openapi.yml
- filename: fieldguide-files-api-openapi.yml
  format: yaml
  label: Fieldguide files API
  slug: fieldguide-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fieldguide/refs/heads/main/openapi/fieldguide-files-api-openapi.yml
- filename: fieldguide-insights-api-openapi.yml
  format: yaml
  label: Fieldguide insights API
  slug: fieldguide-insights-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fieldguide/refs/heads/main/openapi/fieldguide-insights-api-openapi.yml
- filename: fieldguide-jobs-api-openapi.yml
  format: yaml
  label: Fieldguide jobs API
  slug: fieldguide-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fieldguide/refs/heads/main/openapi/fieldguide-jobs-api-openapi.yml
- filename: fieldguide-milestones-api-openapi.yml
  format: yaml
  label: Fieldguide milestones API
  slug: fieldguide-milestones-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fieldguide/refs/heads/main/openapi/fieldguide-milestones-api-openapi.yml
- filename: fieldguide-requests-api-openapi.yml
  format: yaml
  label: Fieldguide requests API
  slug: fieldguide-requests-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fieldguide/refs/heads/main/openapi/fieldguide-requests-api-openapi.yml
- filename: fieldguide-sheet-columns-api-openapi.yml
  format: yaml
  label: Fieldguide sheet-columns API
  slug: fieldguide-sheet-columns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fieldguide/refs/heads/main/openapi/fieldguide-sheet-columns-api-openapi.yml
- filename: fieldguide-sheet-rows-api-openapi.yml
  format: yaml
  label: Fieldguide sheet-rows API
  slug: fieldguide-sheet-rows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fieldguide/refs/heads/main/openapi/fieldguide-sheet-rows-api-openapi.yml
- filename: fieldguide-sheets-api-openapi.yml
  format: yaml
  label: Fieldguide sheets API
  slug: fieldguide-sheets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fieldguide/refs/heads/main/openapi/fieldguide-sheets-api-openapi.yml
- filename: fieldguide-users-api-openapi.yml
  format: yaml
  label: Fieldguide users API
  slug: fieldguide-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fieldguide/refs/heads/main/openapi/fieldguide-users-api-openapi.yml
- filename: fieldguide-webhooks-api-openapi.yml
  format: yaml
  label: Fieldguide webhooks API
  slug: fieldguide-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fieldguide/refs/heads/main/openapi/fieldguide-webhooks-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: fieldguide.io
  spf: true
hosts:
- cert_expires: Sep  6 14:53:35 2026 GMT
  host: www.fieldguide.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 30 13:19:33 2026 GMT
  host: api.fieldguide.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Fieldguide Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Fieldguide, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Fieldguide
provider_slug: fieldguide
slug: fieldguide-domain-security
source_filename: fieldguide-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.fieldguide.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  6 14:53:35 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.fieldguide.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 13:19:33 2026 GMT\n  hsts: null\ndomains:\n- domain: fieldguide.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fieldguide/refs/heads/main/security/fieldguide-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Audit
- Advisory
- Accounting
- Compliance
- Risk
- Engagement Management
- Artificial Intelligence
- Agents
- Webhook
---
