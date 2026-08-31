---
api_specs:
- filename: athenian-align-api-openapi.yml
  format: yaml
  label: Athenian align API
  slug: athenian-align-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/athenian/refs/heads/main/openapi/athenian-align-api-openapi.yml
- filename: athenian-events-api-openapi.yml
  format: yaml
  label: Athenian events API
  slug: athenian-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/athenian/refs/heads/main/openapi/athenian-events-api-openapi.yml
- filename: athenian-filter-api-openapi.yml
  format: yaml
  label: Athenian filter API
  slug: athenian-filter-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/athenian/refs/heads/main/openapi/athenian-filter-api-openapi.yml
- filename: athenian-get-api-openapi.yml
  format: yaml
  label: Athenian get API
  slug: athenian-get-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/athenian/refs/heads/main/openapi/athenian-get-api-openapi.yml
- filename: athenian-histograms-api-openapi.yml
  format: yaml
  label: Athenian histograms API
  slug: athenian-histograms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/athenian/refs/heads/main/openapi/athenian-histograms-api-openapi.yml
- filename: athenian-integrations-api-openapi.yml
  format: yaml
  label: Athenian integrations API
  slug: athenian-integrations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/athenian/refs/heads/main/openapi/athenian-integrations-api-openapi.yml
- filename: athenian-metrics-api-openapi.yml
  format: yaml
  label: Athenian metrics API
  slug: athenian-metrics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/athenian/refs/heads/main/openapi/athenian-metrics-api-openapi.yml
- filename: athenian-pagination-api-openapi.yml
  format: yaml
  label: Athenian pagination API
  slug: athenian-pagination-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/athenian/refs/heads/main/openapi/athenian-pagination-api-openapi.yml
- filename: athenian-registration-api-openapi.yml
  format: yaml
  label: Athenian registration API
  slug: athenian-registration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/athenian/refs/heads/main/openapi/athenian-registration-api-openapi.yml
- filename: athenian-reposet-api-openapi.yml
  format: yaml
  label: Athenian reposet API
  slug: athenian-reposet-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/athenian/refs/heads/main/openapi/athenian-reposet-api-openapi.yml
- filename: athenian-security-api-openapi.yml
  format: yaml
  label: Athenian security API
  slug: athenian-security-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/athenian/refs/heads/main/openapi/athenian-security-api-openapi.yml
- filename: athenian-settings-api-openapi.yml
  format: yaml
  label: Athenian settings API
  slug: athenian-settings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/athenian/refs/heads/main/openapi/athenian-settings-api-openapi.yml
- filename: athenian-team-api-openapi.yml
  format: yaml
  label: Athenian team API
  slug: athenian-team-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/athenian/refs/heads/main/openapi/athenian-team-api-openapi.yml
- filename: athenian-user-api-openapi.yml
  format: yaml
  label: Athenian user API
  slug: athenian-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/athenian/refs/heads/main/openapi/athenian-user-api-openapi.yml
- filename: athenian-version-api-openapi.yml
  format: yaml
  label: Athenian version API
  slug: athenian-version-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/athenian/refs/heads/main/openapi/athenian-version-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: athenian.com
  spf: true
hosts:
- cert_expires: Sep 24 10:43:36 2026 GMT
  host: athenian.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Athenian Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Athenian, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Athenian
provider_slug: athenian
slug: athenian-domain-security
source_filename: athenian-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: athenian.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 10:43:36 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: athenian.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/athenian/refs/heads/main/security/athenian-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Engineering Intelligence
- Software Development Analytics
- Developer Productivity
- DevOps
- Metrics
- Git
- Jira
- CI/CD
- Analytics
---
