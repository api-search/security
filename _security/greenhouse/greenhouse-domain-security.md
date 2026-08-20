---
api_specs:
- filename: greenhouse-applications-api-openapi.yml
  format: yaml
  label: Greenhouse Applications API
  slug: greenhouse-applications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/greenhouse/refs/heads/main/openapi/greenhouse-applications-api-openapi.yml
- filename: greenhouse-candidates-api-openapi.yml
  format: yaml
  label: Greenhouse Candidates API
  slug: greenhouse-candidates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/greenhouse/refs/heads/main/openapi/greenhouse-candidates-api-openapi.yml
- filename: greenhouse-departments-api-openapi.yml
  format: yaml
  label: Greenhouse Departments API
  slug: greenhouse-departments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/greenhouse/refs/heads/main/openapi/greenhouse-departments-api-openapi.yml
- filename: greenhouse-education-api-openapi.yml
  format: yaml
  label: Greenhouse Education API
  slug: greenhouse-education-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/greenhouse/refs/heads/main/openapi/greenhouse-education-api-openapi.yml
- filename: greenhouse-graphql-api-openapi.yml
  format: yaml
  label: Greenhouse Graphql API
  slug: greenhouse-graphql-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/greenhouse/refs/heads/main/openapi/greenhouse-graphql-api-openapi.yml
- filename: greenhouse-greenhouse-job-board-api-api-openapi.yml
  format: yaml
  label: Greenhouse Greenhouse Job Board API API
  slug: greenhouse-greenhouse-job-board-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/greenhouse/refs/heads/main/openapi/greenhouse-greenhouse-job-board-api-api-openapi.yml
- filename: greenhouse-jobs-api-openapi.yml
  format: yaml
  label: Greenhouse Jobs API
  slug: greenhouse-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/greenhouse/refs/heads/main/openapi/greenhouse-jobs-api-openapi.yml
- filename: greenhouse-offices-api-openapi.yml
  format: yaml
  label: Greenhouse Offices API
  slug: greenhouse-offices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/greenhouse/refs/heads/main/openapi/greenhouse-offices-api-openapi.yml
- filename: greenhouse-prospects-api-openapi.yml
  format: yaml
  label: Greenhouse Prospects API
  slug: greenhouse-prospects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/greenhouse/refs/heads/main/openapi/greenhouse-prospects-api-openapi.yml
- filename: greenhouse-sections-api-openapi.yml
  format: yaml
  label: Greenhouse Sections API
  slug: greenhouse-sections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/greenhouse/refs/heads/main/openapi/greenhouse-sections-api-openapi.yml
- filename: greenhouse-tracking-api-openapi.yml
  format: yaml
  label: Greenhouse Tracking API
  slug: greenhouse-tracking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/greenhouse/refs/heads/main/openapi/greenhouse-tracking-api-openapi.yml
- filename: greenhouse-users-api-openapi.yml
  format: yaml
  label: Greenhouse Users API
  slug: greenhouse-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/greenhouse/refs/heads/main/openapi/greenhouse-users-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com"
  - 0 issue "globalsign.com"
  - 0 issue "godaddy.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: greenhouse.io
  spf: true
hosts:
- cert_expires: Sep 11 23:59:59 2026 GMT
  host: developers.greenhouse.io
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 17 23:59:59 2026 GMT
  host: harvest.greenhouse.io
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 17 23:59:59 2026 GMT
  host: boards-api.greenhouse.io
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Greenhouse Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Greenhouse, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Greenhouse
provider_slug: greenhouse
slug: greenhouse-domain-security
source_filename: greenhouse-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developers.greenhouse.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 11 23:59:59 2026 GMT\n  hsts: false\n- host: harvest.greenhouse.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 17 23:59:59 2026 GMT\n  hsts: null\n- host: boards-api.greenhouse.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 17 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: greenhouse.io\n  dnssec: false\n  caa:\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"globalsign.com\"\n  - 0 issue \"godaddy.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/greenhouse/refs/heads/main/security/greenhouse-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- ATS
- Recruiting
- Candidates
- Job
- Onboarding
- HR
---
