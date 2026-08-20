---
api_specs:
- filename: workday-recruiting-agentdefinition-api-openapi.yml
  format: yaml
  label: Workday Recruiting agentDefinition API
  slug: workday-recruiting-agentdefinition-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday-recruiting/refs/heads/main/openapi/workday-recruiting-agentdefinition-api-openapi.yml
- filename: workday-recruiting-applicants-api-openapi.yml
  format: yaml
  label: Workday Recruiting Applicants API
  slug: workday-recruiting-applicants-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday-recruiting/refs/heads/main/openapi/workday-recruiting-applicants-api-openapi.yml
- filename: workday-recruiting-background-checks-api-openapi.yml
  format: yaml
  label: Workday Recruiting Background Checks API
  slug: workday-recruiting-background-checks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday-recruiting/refs/heads/main/openapi/workday-recruiting-background-checks-api-openapi.yml
- filename: workday-recruiting-candidates-api-openapi.yml
  format: yaml
  label: Workday Recruiting Candidates API
  slug: workday-recruiting-candidates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday-recruiting/refs/heads/main/openapi/workday-recruiting-candidates-api-openapi.yml
- filename: workday-recruiting-configuration-api-openapi.yml
  format: yaml
  label: Workday Recruiting Configuration API
  slug: workday-recruiting-configuration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday-recruiting/refs/heads/main/openapi/workday-recruiting-configuration-api-openapi.yml
- filename: workday-recruiting-evergreen-requisitions-api-openapi.yml
  format: yaml
  label: Workday Recruiting Evergreen Requisitions API
  slug: workday-recruiting-evergreen-requisitions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday-recruiting/refs/heads/main/openapi/workday-recruiting-evergreen-requisitions-api-openapi.yml
- filename: workday-recruiting-interviews-api-openapi.yml
  format: yaml
  label: Workday Recruiting Interviews API
  slug: workday-recruiting-interviews-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday-recruiting/refs/heads/main/openapi/workday-recruiting-interviews-api-openapi.yml
- filename: workday-recruiting-job-applications-api-openapi.yml
  format: yaml
  label: Workday Recruiting Job Applications API
  slug: workday-recruiting-job-applications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday-recruiting/refs/heads/main/openapi/workday-recruiting-job-applications-api-openapi.yml
- filename: workday-recruiting-job-postings-api-openapi.yml
  format: yaml
  label: Workday Recruiting Job Postings API
  slug: workday-recruiting-job-postings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday-recruiting/refs/heads/main/openapi/workday-recruiting-job-postings-api-openapi.yml
- filename: workday-recruiting-job-requisitions-api-openapi.yml
  format: yaml
  label: Workday Recruiting Job Requisitions API
  slug: workday-recruiting-job-requisitions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday-recruiting/refs/heads/main/openapi/workday-recruiting-job-requisitions-api-openapi.yml
- filename: workday-recruiting-positions-api-openapi.yml
  format: yaml
  label: Workday Recruiting Positions API
  slug: workday-recruiting-positions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday-recruiting/refs/heads/main/openapi/workday-recruiting-positions-api-openapi.yml
- filename: workday-recruiting-recruiting-agencies-api-openapi.yml
  format: yaml
  label: Workday Recruiting Recruiting Agencies API
  slug: workday-recruiting-recruiting-agencies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday-recruiting/refs/heads/main/openapi/workday-recruiting-recruiting-agencies-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: workday.com
  spf: true
hosts:
- cert_expires: Sep 10 23:59:59 2026 GMT
  host: community.workday.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  2 03:30:49 2026 GMT
  host: wd2-impl-services1.workday.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Workday Recruiting Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Workday Recruiting, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Workday Recruiting
provider_slug: workday-recruiting
slug: workday-recruiting-domain-security
source_filename: workday-recruiting-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: community.workday.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 10 23:59:59 2026 GMT\n  hsts: null\n- host: wd2-impl-services1.workday.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  2 03:30:49 2026 GMT\n  hsts: null\ndomains:\n- domain: workday.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/workday-recruiting/refs/heads/main/security/workday-recruiting-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- HCM
- Human Resources
- Recruiting
- Software-as-a-Service
- Talent Acquisition
---
