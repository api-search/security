---
api_specs:
- filename: avoma-calls-api-openapi.yml
  format: yaml
  label: Avoma Calls API
  slug: avoma-calls-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/avoma/refs/heads/main/openapi/avoma-calls-api-openapi.yml
- filename: avoma-custom-category-api-openapi.yml
  format: yaml
  label: Avoma Custom Category API
  slug: avoma-custom-category-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/avoma/refs/heads/main/openapi/avoma-custom-category-api-openapi.yml
- filename: avoma-engagement-analytics-api-openapi.yml
  format: yaml
  label: Avoma Engagement Analytics API
  slug: avoma-engagement-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/avoma/refs/heads/main/openapi/avoma-engagement-analytics-api-openapi.yml
- filename: avoma-meeting-outcomes-api-openapi.yml
  format: yaml
  label: Avoma Meeting Outcomes API
  slug: avoma-meeting-outcomes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/avoma/refs/heads/main/openapi/avoma-meeting-outcomes-api-openapi.yml
- filename: avoma-meeting-types-api-openapi.yml
  format: yaml
  label: Avoma Meeting Types API
  slug: avoma-meeting-types-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/avoma/refs/heads/main/openapi/avoma-meeting-types-api-openapi.yml
- filename: avoma-meetings-api-openapi.yml
  format: yaml
  label: Avoma Meetings API
  slug: avoma-meetings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/avoma/refs/heads/main/openapi/avoma-meetings-api-openapi.yml
- filename: avoma-meetings-sentiments-api-openapi.yml
  format: yaml
  label: Avoma Meetings Sentiments API
  slug: avoma-meetings-sentiments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/avoma/refs/heads/main/openapi/avoma-meetings-sentiments-api-openapi.yml
- filename: avoma-notes-api-openapi.yml
  format: yaml
  label: Avoma Notes API
  slug: avoma-notes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/avoma/refs/heads/main/openapi/avoma-notes-api-openapi.yml
- filename: avoma-recording-api-openapi.yml
  format: yaml
  label: Avoma Recording API
  slug: avoma-recording-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/avoma/refs/heads/main/openapi/avoma-recording-api-openapi.yml
- filename: avoma-revenue-intelligence-beta-api-openapi.yml
  format: yaml
  label: Avoma Revenue Intelligence [Beta] API
  slug: avoma-revenue-intelligence-beta-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/avoma/refs/heads/main/openapi/avoma-revenue-intelligence-beta-api-openapi.yml
- filename: avoma-scorecard-evaluations-api-openapi.yml
  format: yaml
  label: Avoma Scorecard Evaluations API
  slug: avoma-scorecard-evaluations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/avoma/refs/heads/main/openapi/avoma-scorecard-evaluations-api-openapi.yml
- filename: avoma-scorecards-api-openapi.yml
  format: yaml
  label: Avoma Scorecards API
  slug: avoma-scorecards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/avoma/refs/heads/main/openapi/avoma-scorecards-api-openapi.yml
- filename: avoma-smart-category-api-openapi.yml
  format: yaml
  label: Avoma Smart Category API
  slug: avoma-smart-category-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/avoma/refs/heads/main/openapi/avoma-smart-category-api-openapi.yml
- filename: avoma-snippets-api-openapi.yml
  format: yaml
  label: Avoma Snippets API
  slug: avoma-snippets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/avoma/refs/heads/main/openapi/avoma-snippets-api-openapi.yml
- filename: avoma-templates-api-openapi.yml
  format: yaml
  label: Avoma Templates API
  slug: avoma-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/avoma/refs/heads/main/openapi/avoma-templates-api-openapi.yml
- filename: avoma-transcriptions-api-openapi.yml
  format: yaml
  label: Avoma Transcriptions API
  slug: avoma-transcriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/avoma/refs/heads/main/openapi/avoma-transcriptions-api-openapi.yml
- filename: avoma-users-api-openapi.yml
  format: yaml
  label: Avoma Users API
  slug: avoma-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/avoma/refs/heads/main/openapi/avoma-users-api-openapi.yml
- filename: avoma-webhooks-api-openapi.yml
  format: yaml
  label: Avoma Webhooks API
  slug: avoma-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/avoma/refs/heads/main/openapi/avoma-webhooks-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: avoma.com
  spf: true
hosts:
- cert_expires: Dec 12 11:28:13 2026 GMT
  host: www.avoma.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Avoma Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Avoma, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Avoma
provider_slug: avoma
slug: avoma-domain-security
source_filename: avoma-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.avoma.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 12 11:28:13 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: avoma.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/avoma/refs/heads/main/security/avoma-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Artificial Intelligence
- Meeting Assistant
- Sales Enablement
- Automation
- Productivity
---
