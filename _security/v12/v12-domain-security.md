---
api_specs:
- filename: v12-documents-api-openapi.yml
  format: yaml
  label: V12 Documents API
  slug: v12-documents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/v12/openapi/v12-documents-api-openapi.yml
- filename: v12-findings-api-openapi.yml
  format: yaml
  label: V12 Findings API
  slug: v12-findings-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/v12/openapi/v12-findings-api-openapi.yml
- filename: v12-me-api-openapi.yml
  format: yaml
  label: V12 Me API
  slug: v12-me-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/v12/openapi/v12-me-api-openapi.yml
- filename: v12-members-api-openapi.yml
  format: yaml
  label: V12 Members API
  slug: v12-members-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/v12/openapi/v12-members-api-openapi.yml
- filename: v12-repositories-api-openapi.yml
  format: yaml
  label: V12 Repositories API
  slug: v12-repositories-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/v12/openapi/v12-repositories-api-openapi.yml
- filename: v12-runs-api-openapi.yml
  format: yaml
  label: V12 Runs API
  slug: v12-runs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/v12/openapi/v12-runs-api-openapi.yml
- filename: v12-steers-api-openapi.yml
  format: yaml
  label: V12 Steers API
  slug: v12-steers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/v12/openapi/v12-steers-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: v12.sh
  spf: true
hosts:
- cert_expires: Nov 27 05:28:17 2026 GMT
  host: v12.sh
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: V12 Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for V12, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: V12
provider_slug: v12
slug: v12-domain-security
source_filename: v12-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: v12.sh\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 27 05:28:17 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: v12.sh\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/v12/security/v12-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Security
- DevOps
- Automation
- Code Analysis
---
