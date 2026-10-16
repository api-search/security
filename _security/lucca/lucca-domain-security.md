---
api_specs:
- filename: lucca-employee-attributes-api-openapi.yml
  format: yaml
  label: Lucca Employee Attributes API
  slug: lucca-employee-attributes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lucca/refs/heads/main/openapi/lucca-employee-attributes-api-openapi.yml
- filename: lucca-employee-job-qualifications-api-openapi.yml
  format: yaml
  label: Lucca Employee Job Qualifications API
  slug: lucca-employee-job-qualifications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lucca/refs/heads/main/openapi/lucca-employee-job-qualifications-api-openapi.yml
- filename: lucca-employee-occupation-categories-api-openapi.yml
  format: yaml
  label: Lucca Employee Occupation Categories API
  slug: lucca-employee-occupation-categories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lucca/refs/heads/main/openapi/lucca-employee-occupation-categories-api-openapi.yml
- filename: lucca-employees-api-openapi.yml
  format: yaml
  label: Lucca Employees API
  slug: lucca-employees-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lucca/refs/heads/main/openapi/lucca-employees-api-openapi.yml
- filename: lucca-employments-api-openapi.yml
  format: yaml
  label: Lucca Employments API
  slug: lucca-employments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lucca/refs/heads/main/openapi/lucca-employments-api-openapi.yml
- filename: lucca-events-api-openapi.yml
  format: yaml
  label: Lucca Events API
  slug: lucca-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lucca/refs/heads/main/openapi/lucca-events-api-openapi.yml
- filename: lucca-files-api-openapi.yml
  format: yaml
  label: Lucca Files API
  slug: lucca-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lucca/refs/heads/main/openapi/lucca-files-api-openapi.yml
- filename: lucca-organization-api-openapi.yml
  format: yaml
  label: Lucca Organization API
  slug: lucca-organization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lucca/refs/heads/main/openapi/lucca-organization-api-openapi.yml
- filename: lucca-taxonomies-api-openapi.yml
  format: yaml
  label: Lucca Taxonomies API
  slug: lucca-taxonomies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lucca/refs/heads/main/openapi/lucca-taxonomies-api-openapi.yml
- filename: lucca-webhooks-api-openapi.yml
  format: yaml
  label: Lucca Webhooks API
  slug: lucca-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lucca/refs/heads/main/openapi/lucca-webhooks-api-openapi.yml
- filename: lucca-working-time-arrangements-api-openapi.yml
  format: yaml
  label: Lucca Working Time Arrangements API
  slug: lucca-working-time-arrangements-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lucca/refs/heads/main/openapi/lucca-working-time-arrangements-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: lucca.fr
  spf: true
hosts:
- cert_expires: Nov 15 00:15:18 2026 GMT
  host: www.lucca.fr
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Lucca Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Lucca, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Lucca
provider_slug: lucca
slug: lucca-domain-security
source_filename: lucca-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-14'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.lucca.fr\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 15 00:15:18 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\ndomains:\n- domain: lucca.fr\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lucca/refs/heads/main/security/lucca-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- HR
- SaaS
- Payroll
- Talent Management
---
