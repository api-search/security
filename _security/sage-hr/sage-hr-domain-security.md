---
api_specs:
- filename: sage-hr-documents-api-openapi.yml
  format: yaml
  label: Sage HR Documents API
  slug: sage-hr-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sage-hr/refs/heads/main/openapi/sage-hr-documents-api-openapi.yml
- filename: sage-hr-employee-api-openapi.yml
  format: yaml
  label: Sage HR Employee API
  slug: sage-hr-employee-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sage-hr/refs/heads/main/openapi/sage-hr-employee-api-openapi.yml
- filename: sage-hr-integrations-api-openapi.yml
  format: yaml
  label: Sage HR Integrations API
  slug: sage-hr-integrations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sage-hr/refs/heads/main/openapi/sage-hr-integrations-api-openapi.yml
- filename: sage-hr-kit-days-api-openapi.yml
  format: yaml
  label: Sage HR KIT days API
  slug: sage-hr-kit-days-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sage-hr/refs/heads/main/openapi/sage-hr-kit-days-api-openapi.yml
- filename: sage-hr-leave-management-api-openapi.yml
  format: yaml
  label: Sage HR Leave management API
  slug: sage-hr-leave-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sage-hr/refs/heads/main/openapi/sage-hr-leave-management-api-openapi.yml
- filename: sage-hr-offboarding-api-openapi.yml
  format: yaml
  label: Sage HR Offboarding API
  slug: sage-hr-offboarding-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sage-hr/refs/heads/main/openapi/sage-hr-offboarding-api-openapi.yml
- filename: sage-hr-onboarding-api-openapi.yml
  format: yaml
  label: Sage HR Onboarding API
  slug: sage-hr-onboarding-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sage-hr/refs/heads/main/openapi/sage-hr-onboarding-api-openapi.yml
- filename: sage-hr-performance-api-openapi.yml
  format: yaml
  label: Sage HR Performance API
  slug: sage-hr-performance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sage-hr/refs/heads/main/openapi/sage-hr-performance-api-openapi.yml
- filename: sage-hr-policies-api-openapi.yml
  format: yaml
  label: Sage HR Policies API
  slug: sage-hr-policies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sage-hr/refs/heads/main/openapi/sage-hr-policies-api-openapi.yml
- filename: sage-hr-positions-api-openapi.yml
  format: yaml
  label: Sage HR Positions API
  slug: sage-hr-positions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sage-hr/refs/heads/main/openapi/sage-hr-positions-api-openapi.yml
- filename: sage-hr-recruitment-api-openapi.yml
  format: yaml
  label: Sage HR Recruitment API
  slug: sage-hr-recruitment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sage-hr/refs/heads/main/openapi/sage-hr-recruitment-api-openapi.yml
- filename: sage-hr-teams-api-openapi.yml
  format: yaml
  label: Sage HR Teams API
  slug: sage-hr-teams-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sage-hr/refs/heads/main/openapi/sage-hr-teams-api-openapi.yml
- filename: sage-hr-terminations-reasons-api-openapi.yml
  format: yaml
  label: Sage HR Terminations reasons API
  slug: sage-hr-terminations-reasons-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sage-hr/refs/heads/main/openapi/sage-hr-terminations-reasons-api-openapi.yml
- filename: sage-hr-timesheets-api-openapi.yml
  format: yaml
  label: Sage HR Timesheets API
  slug: sage-hr-timesheets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sage-hr/refs/heads/main/openapi/sage-hr-timesheets-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: sage.hr
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: sage.com
  spf: true
hosts:
- cert_expires: Sep  3 12:35:52 2026 GMT
  host: sage.hr
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 10 23:59:59 2026 GMT
  host: www.sage.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  3 12:35:52 2026 GMT
  host: apidoc.sage.hr
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Sage Hr Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Sage HR, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Sage HR
provider_slug: sage-hr
slug: sage-hr-domain-security
source_filename: sage-hr-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: sage.hr\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  3 12:35:52 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: www.sage.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 10 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: apidoc.sage.hr\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  3 12:35:52 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: sage.hr\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: sage.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sage-hr/refs/heads/main/security/sage-hr-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- HR
- HRIS
- People
- SMB
- Leave Management
- Recruitment
- Performance
- Timesheets
- Onboarding
---
