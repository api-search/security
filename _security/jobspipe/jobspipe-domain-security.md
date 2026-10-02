---
api_specs:
- filename: jobspipe-account-api-openapi.yml
  format: yaml
  label: JobsPipe Account API
  slug: jobspipe-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jobspipe/refs/heads/main/openapi/jobspipe-account-api-openapi.yml
- filename: jobspipe-billing-api-openapi.yml
  format: yaml
  label: JobsPipe Billing API
  slug: jobspipe-billing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jobspipe/refs/heads/main/openapi/jobspipe-billing-api-openapi.yml
- filename: jobspipe-companies-api-openapi.yml
  format: yaml
  label: JobsPipe Companies API
  slug: jobspipe-companies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jobspipe/refs/heads/main/openapi/jobspipe-companies-api-openapi.yml
- filename: jobspipe-jobs-api-openapi.yml
  format: yaml
  label: JobsPipe Jobs API
  slug: jobspipe-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jobspipe/refs/heads/main/openapi/jobspipe-jobs-api-openapi.yml
- filename: jobspipe-jobspipe-api-api-openapi.yml
  format: yaml
  label: JobsPipe JobsPipe API
  slug: jobspipe-jobspipe-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jobspipe/refs/heads/main/openapi/jobspipe-jobspipe-api-api-openapi.yml
- filename: jobspipe-labour-market-insights-api-openapi.yml
  format: yaml
  label: JobsPipe Labour Market Insights API
  slug: jobspipe-labour-market-insights-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jobspipe/refs/heads/main/openapi/jobspipe-labour-market-insights-api-openapi.yml
- filename: jobspipe-monitors-api-openapi.yml
  format: yaml
  label: JobsPipe Monitors API
  slug: jobspipe-monitors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jobspipe/refs/heads/main/openapi/jobspipe-monitors-api-openapi.yml
- filename: jobspipe-sandbox-api-openapi.yml
  format: yaml
  label: JobsPipe Sandbox API
  slug: jobspipe-sandbox-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jobspipe/refs/heads/main/openapi/jobspipe-sandbox-api-openapi.yml
- filename: jobspipe-stack-api-openapi.yml
  format: yaml
  label: JobsPipe Stack API
  slug: jobspipe-stack-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jobspipe/refs/heads/main/openapi/jobspipe-stack-api-openapi.yml
- filename: jobspipe-technologies-api-openapi.yml
  format: yaml
  label: JobsPipe Technologies API
  slug: jobspipe-technologies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jobspipe/refs/heads/main/openapi/jobspipe-technologies-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: jobspipe.dev
  spf: true
hosts:
- cert_expires: Dec  3 08:48:08 2026 GMT
  host: jobspipe.dev
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Jobspipe Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for JobsPipe, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: JobsPipe
provider_slug: jobspipe
slug: jobspipe-domain-security
source_filename: jobspipe-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: jobspipe.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  3 08:48:08 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: jobspipe.dev\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/jobspipe/refs/heads/main/security/jobspipe-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Jobs
- API
- Data
- Hiring
---
