---
api_specs:
- filename: kondukto-authorization-managers-api-openapi.yml
  format: yaml
  label: Kondukto Authorization Managers API
  slug: kondukto-authorization-managers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kondukto/refs/heads/main/openapi/kondukto-authorization-managers-api-openapi.yml
- filename: kondukto-events-api-openapi.yml
  format: yaml
  label: Kondukto Events API
  slug: kondukto-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kondukto/refs/heads/main/openapi/kondukto-events-api-openapi.yml
- filename: kondukto-health-api-openapi.yml
  format: yaml
  label: Kondukto Health API
  slug: kondukto-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kondukto/refs/heads/main/openapi/kondukto-health-api-openapi.yml
- filename: kondukto-labels-api-openapi.yml
  format: yaml
  label: Kondukto Labels API
  slug: kondukto-labels-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kondukto/refs/heads/main/openapi/kondukto-labels-api-openapi.yml
- filename: kondukto-products-api-openapi.yml
  format: yaml
  label: Kondukto Products API
  slug: kondukto-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kondukto/refs/heads/main/openapi/kondukto-products-api-openapi.yml
- filename: kondukto-projects-api-openapi.yml
  format: yaml
  label: Kondukto Projects API
  slug: kondukto-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kondukto/refs/heads/main/openapi/kondukto-projects-api-openapi.yml
- filename: kondukto-scanners-api-openapi.yml
  format: yaml
  label: Kondukto Scanners API
  slug: kondukto-scanners-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kondukto/refs/heads/main/openapi/kondukto-scanners-api-openapi.yml
- filename: kondukto-scans-api-openapi.yml
  format: yaml
  label: Kondukto Scans API
  slug: kondukto-scans-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kondukto/refs/heads/main/openapi/kondukto-scans-api-openapi.yml
- filename: kondukto-teams-api-openapi.yml
  format: yaml
  label: Kondukto Teams API
  slug: kondukto-teams-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kondukto/refs/heads/main/openapi/kondukto-teams-api-openapi.yml
- filename: kondukto-users-api-openapi.yml
  format: yaml
  label: Kondukto Users API
  slug: kondukto-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kondukto/refs/heads/main/openapi/kondukto-users-api-openapi.yml
- filename: kondukto-vulnerabilities-api-openapi.yml
  format: yaml
  label: Kondukto Vulnerabilities API
  slug: kondukto-vulnerabilities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kondukto/refs/heads/main/openapi/kondukto-vulnerabilities-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: kondukto.io
  spf: true
hosts:
- cert_expires: Sep 23 22:10:03 2026 GMT
  host: kondukto.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 24 02:11:29 2026 GMT
  host: docs.kondukto.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 24 23:59:59 2026 GMT
  host: api.kondukto.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Kondukto Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Kondukto, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Kondukto
provider_slug: kondukto
slug: kondukto-domain-security
source_filename: kondukto-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: kondukto.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 22:10:03 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.kondukto.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 02:11:29 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.kondukto.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: kondukto.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kondukto/refs/heads/main/security/kondukto-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Application Security
- ASPM
- Vulnerability Management
- DevSecOps
- Security Orchestration
- SAST
- DAST
- SCA
- Software Composition Analysis
- Container Security
- SBOM
- Security Testing
- CI/CD
- Security
---
