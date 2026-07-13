---
api_specs:
- filename: assembled-people-api-openapi.yml
  format: yaml
  label: Assembled People API
  slug: assembled-people-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/assembled/refs/heads/main/openapi/assembled-people-api-openapi.yml
- filename: assembled-agent-state-api-openapi.yml
  format: yaml
  label: Assembled Agent State API
  slug: assembled-agent-state-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/assembled/refs/heads/main/openapi/assembled-agent-state-api-openapi.yml
- filename: assembled-activities-api-openapi.yml
  format: yaml
  label: Assembled Activities API
  slug: assembled-activities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/assembled/refs/heads/main/openapi/assembled-activities-api-openapi.yml
- filename: assembled-filters-api-openapi.yml
  format: yaml
  label: Assembled Filters API
  slug: assembled-filters-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/assembled/refs/heads/main/openapi/assembled-filters-api-openapi.yml
- filename: assembled-forecasts-api-openapi.yml
  format: yaml
  label: Assembled Forecasts API
  slug: assembled-forecasts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/assembled/refs/heads/main/openapi/assembled-forecasts-api-openapi.yml
- filename: assembled-time-off-api-openapi.yml
  format: yaml
  label: Assembled Time Off API
  slug: assembled-time-off-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/assembled/refs/heads/main/openapi/assembled-time-off-api-openapi.yml
- filename: assembled-requirements-api-openapi.yml
  format: yaml
  label: Assembled Requirements API
  slug: assembled-requirements-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/assembled/refs/heads/main/openapi/assembled-requirements-api-openapi.yml
- filename: assembled-scheduling-rules-api-openapi.yml
  format: yaml
  label: Assembled Scheduling Rules API
  slug: assembled-scheduling-rules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/assembled/refs/heads/main/openapi/assembled-scheduling-rules-api-openapi.yml
- filename: assembled-conversations-api-openapi.yml
  format: yaml
  label: Assembled Conversations API
  slug: assembled-conversations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/assembled/refs/heads/main/openapi/assembled-conversations-api-openapi.yml
- filename: assembled-reports-api-openapi.yml
  format: yaml
  label: Assembled Reports API
  slug: assembled-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/assembled/refs/heads/main/openapi/assembled-reports-api-openapi.yml
- filename: assembled-qa-api-openapi.yml
  format: yaml
  label: Assembled QA API
  slug: assembled-qa-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/assembled/refs/heads/main/openapi/assembled-qa-api-openapi.yml
- filename: assembled-assist-api-openapi.yml
  format: yaml
  label: Assembled Assist API
  slug: assembled-assist-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/assembled/refs/heads/main/openapi/assembled-assist-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: assembled.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: assembledhq.com
  spf: true
hosts:
- cert_expires: Sep  9 17:55:31 2026 GMT
  host: www.assembled.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 27 04:16:49 2026 GMT
  host: docs.assembled.com
  hsts: true
  hsts_max_age: 31556952
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 20 23:59:59 2026 GMT
  host: api.assembledhq.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Assembled Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Assembled, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Assembled
provider_slug: assembled
slug: assembled-domain-security
source_filename: assembled-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.assembled.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  9 17:55:31 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.assembled.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 27 04:16:49 2026 GMT\n  hsts: true\n  hsts_max_age: 31556952\n- host: api.assembledhq.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov 20 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: assembled.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: assembledhq.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/assembled/refs/heads/main/security/assembled-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Customer Support
- Workforce Management
- WFM
- AI Agents
- AI Copilot
- Contact Center
- Customer Experience
- Support Operations
- Scheduling
- Forecasting
- Quality Assurance
- Vendor Management
- BPO
---
