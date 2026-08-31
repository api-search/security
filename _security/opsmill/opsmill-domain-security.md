---
api_specs:
- filename: opsmill-artifact-api-openapi.yml
  format: yaml
  label: OpsMill Artifact API
  slug: opsmill-artifact-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opsmill/refs/heads/main/openapi/opsmill-artifact-api-openapi.yml
- filename: opsmill-auth-api-openapi.yml
  format: yaml
  label: OpsMill Auth API
  slug: opsmill-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opsmill/refs/heads/main/openapi/opsmill-auth-api-openapi.yml
- filename: opsmill-config-api-openapi.yml
  format: yaml
  label: OpsMill Config API
  slug: opsmill-config-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opsmill/refs/heads/main/openapi/opsmill-config-api-openapi.yml
- filename: opsmill-diff-api-openapi.yml
  format: yaml
  label: OpsMill Diff API
  slug: opsmill-diff-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opsmill/refs/heads/main/openapi/opsmill-diff-api-openapi.yml
- filename: opsmill-file-api-openapi.yml
  format: yaml
  label: OpsMill File API
  slug: opsmill-file-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opsmill/refs/heads/main/openapi/opsmill-file-api-openapi.yml
- filename: opsmill-info-api-openapi.yml
  format: yaml
  label: OpsMill Info API
  slug: opsmill-info-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opsmill/refs/heads/main/openapi/opsmill-info-api-openapi.yml
- filename: opsmill-menu-api-openapi.yml
  format: yaml
  label: OpsMill Menu API
  slug: opsmill-menu-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opsmill/refs/heads/main/openapi/opsmill-menu-api-openapi.yml
- filename: opsmill-oauth2-api-openapi.yml
  format: yaml
  label: OpsMill Oauth2 API
  slug: opsmill-oauth2-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opsmill/refs/heads/main/openapi/opsmill-oauth2-api-openapi.yml
- filename: opsmill-oidc-api-openapi.yml
  format: yaml
  label: OpsMill Oidc API
  slug: opsmill-oidc-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opsmill/refs/heads/main/openapi/opsmill-oidc-api-openapi.yml
- filename: opsmill-query-api-openapi.yml
  format: yaml
  label: OpsMill Query API
  slug: opsmill-query-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opsmill/refs/heads/main/openapi/opsmill-query-api-openapi.yml
- filename: opsmill-schema-api-openapi.yml
  format: yaml
  label: OpsMill Schema API
  slug: opsmill-schema-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opsmill/refs/heads/main/openapi/opsmill-schema-api-openapi.yml
- filename: opsmill-schema-graphql-api-openapi.yml
  format: yaml
  label: OpsMill Schema.graphql API
  slug: opsmill-schema-graphql-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opsmill/refs/heads/main/openapi/opsmill-schema-graphql-api-openapi.yml
- filename: opsmill-storage-api-openapi.yml
  format: yaml
  label: OpsMill Storage API
  slug: opsmill-storage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opsmill/refs/heads/main/openapi/opsmill-storage-api-openapi.yml
- filename: opsmill-telemetry-api-openapi.yml
  format: yaml
  label: OpsMill Telemetry API
  slug: opsmill-telemetry-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opsmill/refs/heads/main/openapi/opsmill-telemetry-api-openapi.yml
- filename: opsmill-transform-api-openapi.yml
  format: yaml
  label: OpsMill Transform API
  slug: opsmill-transform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opsmill/refs/heads/main/openapi/opsmill-transform-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: opsmill.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: infrahub.app
  spf: false
hosts:
- cert_expires: Aug 30 18:11:12 2026 GMT
  host: opsmill.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  7 15:17:56 2026 GMT
  host: docs.infrahub.app
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  4 02:15:34 2026 GMT
  host: sandbox.infrahub.app
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Opsmill Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for OpsMill, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: OpsMill
provider_slug: opsmill
slug: opsmill-domain-security
source_filename: opsmill-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: opsmill.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 30 18:11:12 2026 GMT\n  hsts: false\n- host: docs.infrahub.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 15:17:56 2026 GMT\n  hsts: false\n- host: sandbox.infrahub.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 02:15:34 2026 GMT\n  hsts: null\ndomains:\n- domain: opsmill.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: infrahub.app\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/opsmill/refs/heads/main/security/opsmill-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Infrastructure Saas
- Network Automation
- Source Of Truth
- Data Management
- GraphQL
- DevOps
- Configuration Management
- AIOps
- Open-Source
---
