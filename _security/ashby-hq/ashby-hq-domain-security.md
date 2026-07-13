---
api_specs:
- filename: ashby-openapi.yml
  format: yaml
  label: Ashby Applications API
  slug: ashby-applications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ashby-hq/refs/heads/main/openapi/ashby-openapi.yml
- filename: ashby-openapi.yml
  format: yaml
  label: Ashby Candidates API
  slug: ashby-candidates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ashby-hq/refs/heads/main/openapi/ashby-openapi.yml
- filename: ashby-openapi.yml
  format: yaml
  label: Ashby Jobs API
  slug: ashby-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ashby-hq/refs/heads/main/openapi/ashby-openapi.yml
- filename: ashby-openapi.yml
  format: yaml
  label: Ashby Interviews API
  slug: ashby-interviews-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ashby-hq/refs/heads/main/openapi/ashby-openapi.yml
- filename: ashby-openapi.yml
  format: yaml
  label: Ashby Offers API
  slug: ashby-offers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ashby-hq/refs/heads/main/openapi/ashby-openapi.yml
- filename: ashby-openapi.yml
  format: yaml
  label: Ashby Approvals API
  slug: ashby-approvals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ashby-hq/refs/heads/main/openapi/ashby-openapi.yml
- filename: ashby-openapi.yml
  format: yaml
  label: Ashby Surveys & Feedback API
  slug: ashby-surveys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ashby-hq/refs/heads/main/openapi/ashby-openapi.yml
- filename: ashby-openapi.yml
  format: yaml
  label: Ashby Assessments API
  slug: ashby-assessments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ashby-hq/refs/heads/main/openapi/ashby-openapi.yml
- filename: ashby-openapi.yml
  format: yaml
  label: Ashby Custom Fields API
  slug: ashby-custom-fields-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ashby-hq/refs/heads/main/openapi/ashby-openapi.yml
- filename: ashby-openapi.yml
  format: yaml
  label: Ashby Organization API
  slug: ashby-organization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ashby-hq/refs/heads/main/openapi/ashby-openapi.yml
- filename: ashby-openapi.yml
  format: yaml
  label: Ashby Files API
  slug: ashby-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ashby-hq/refs/heads/main/openapi/ashby-openapi.yml
- filename: ashby-openapi.yml
  format: yaml
  label: Ashby Reports API
  slug: ashby-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ashby-hq/refs/heads/main/openapi/ashby-openapi.yml
- filename: ashby-openapi.yml
  format: yaml
  label: Ashby Webhooks API
  slug: ashby-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ashby-hq/refs/heads/main/openapi/ashby-openapi.yml
- filename: ashby-openapi.yml
  format: yaml
  label: Ashby API Keys API
  slug: ashby-api-keys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ashby-hq/refs/heads/main/openapi/ashby-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: ashbyhq.com
  spf: true
hosts:
- cert_expires: Oct  1 20:03:45 2026 GMT
  host: www.ashbyhq.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  2 19:53:45 2026 GMT
  host: developers.ashbyhq.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  3 00:41:00 2026 GMT
  host: api.ashbyhq.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ashby Hq Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ashby, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Ashby
provider_slug: ashby-hq
slug: ashby-hq-domain-security
source_filename: ashby-hq-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.ashbyhq.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 20:03:45 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developers.ashbyhq.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 19:53:45 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.ashbyhq.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 00:41:00 2026 GMT\n  hsts: null\ndomains:\n- domain: ashbyhq.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ashby-hq/refs/heads/main/security/ashby-hq-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- ATS
- Applicant Tracking System
- Recruiting
- Talent Acquisition
- Sourcing
- CRM
- Scheduling
- Analytics
- Hiring
- HR Tech
- AI
---
