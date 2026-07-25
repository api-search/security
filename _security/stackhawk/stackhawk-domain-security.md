---
api_specs:
- filename: stackhawk-api-authentication-api-openapi.yml
  format: yaml
  label: StackHawk Api Authentication API
  slug: stackhawk-api-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stackhawk/refs/heads/main/openapi/stackhawk-api-authentication-api-openapi.yml
- filename: stackhawk-applications-api-openapi.yml
  format: yaml
  label: StackHawk Applications API
  slug: stackhawk-applications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stackhawk/refs/heads/main/openapi/stackhawk-applications-api-openapi.yml
- filename: stackhawk-global-configuration-api-openapi.yml
  format: yaml
  label: StackHawk Global Configuration API
  slug: stackhawk-global-configuration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stackhawk/refs/heads/main/openapi/stackhawk-global-configuration-api-openapi.yml
- filename: stackhawk-hosted-oas-api-openapi.yml
  format: yaml
  label: StackHawk Hosted OAS API
  slug: stackhawk-hosted-oas-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stackhawk/refs/heads/main/openapi/stackhawk-hosted-oas-api-openapi.yml
- filename: stackhawk-organization-teams-api-openapi.yml
  format: yaml
  label: StackHawk Organization Teams API
  slug: stackhawk-organization-teams-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stackhawk/refs/heads/main/openapi/stackhawk-organization-teams-api-openapi.yml
- filename: stackhawk-organizations-api-openapi.yml
  format: yaml
  label: StackHawk Organizations API
  slug: stackhawk-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stackhawk/refs/heads/main/openapi/stackhawk-organizations-api-openapi.yml
- filename: stackhawk-perch-api-openapi.yml
  format: yaml
  label: StackHawk Perch API
  slug: stackhawk-perch-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stackhawk/refs/heads/main/openapi/stackhawk-perch-api-openapi.yml
- filename: stackhawk-profile-scans-api-openapi.yml
  format: yaml
  label: StackHawk Profile Scans API
  slug: stackhawk-profile-scans-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stackhawk/refs/heads/main/openapi/stackhawk-profile-scans-api-openapi.yml
- filename: stackhawk-reports-api-openapi.yml
  format: yaml
  label: StackHawk Reports API
  slug: stackhawk-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stackhawk/refs/heads/main/openapi/stackhawk-reports-api-openapi.yml
- filename: stackhawk-repositories-api-openapi.yml
  format: yaml
  label: StackHawk Repositories API
  slug: stackhawk-repositories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stackhawk/refs/heads/main/openapi/stackhawk-repositories-api-openapi.yml
- filename: stackhawk-scan-configuration-api-openapi.yml
  format: yaml
  label: StackHawk Scan Configuration API
  slug: stackhawk-scan-configuration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stackhawk/refs/heads/main/openapi/stackhawk-scan-configuration-api-openapi.yml
- filename: stackhawk-scan-policies-api-openapi.yml
  format: yaml
  label: StackHawk Scan Policies API
  slug: stackhawk-scan-policies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stackhawk/refs/heads/main/openapi/stackhawk-scan-policies-api-openapi.yml
- filename: stackhawk-scan-results-api-openapi.yml
  format: yaml
  label: StackHawk Scan Results API
  slug: stackhawk-scan-results-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stackhawk/refs/heads/main/openapi/stackhawk-scan-results-api-openapi.yml
- filename: stackhawk-user-api-openapi.yml
  format: yaml
  label: StackHawk User API
  slug: stackhawk-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stackhawk/refs/heads/main/openapi/stackhawk-user-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: stackhawk.com
  spf: true
hosts:
- cert_expires: Oct  4 02:36:05 2026 GMT
  host: www.stackhawk.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 17 19:55:18 2026 GMT
  host: apidocs.stackhawk.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  8 23:59:59 2026 GMT
  host: api.stackhawk.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Stackhawk Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for StackHawk, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: StackHawk
provider_slug: stackhawk
slug: stackhawk-domain-security
source_filename: stackhawk-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.stackhawk.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 02:36:05 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: apidocs.stackhawk.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 17 19:55:18 2026 GMT\n  hsts: null\n- host: api.stackhawk.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec  8 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: stackhawk.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/stackhawk/refs/heads/main/security/stackhawk-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- API Security
- Application Security
- DAST
- Security Testing
- Vulnerability Management
---
