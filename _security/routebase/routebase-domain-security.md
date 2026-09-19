---
api_specs:
- filename: routebase-api-specs-api-openapi.yml
  format: yaml
  label: Routebase API Specs API
  slug: routebase-api-specs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/routebase/refs/heads/main/openapi/routebase-api-specs-api-openapi.yml
- filename: routebase-ci-test-runs-api-openapi.yml
  format: yaml
  label: Routebase CI & Test Runs API
  slug: routebase-ci-test-runs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/routebase/refs/heads/main/openapi/routebase-ci-test-runs-api-openapi.yml
- filename: routebase-docs-as-code-api-openapi.yml
  format: yaml
  label: Routebase Docs as Code API
  slug: routebase-docs-as-code-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/routebase/refs/heads/main/openapi/routebase-docs-as-code-api-openapi.yml
- filename: routebase-scim-api-openapi.yml
  format: yaml
  label: Routebase SCIM API
  slug: routebase-scim-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/routebase/refs/heads/main/openapi/routebase-scim-api-openapi.yml
- filename: routebase-security-api-openapi.yml
  format: yaml
  label: Routebase Security API
  slug: routebase-security-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/routebase/refs/heads/main/openapi/routebase-security-api-openapi.yml
description: ''
domains:
- caa:
  - 0 iodef "mailto:denny.riedl@routebase.dev"
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  - 0 issuewild "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: routebase.dev
  spf: true
hosts:
- cert_expires: Dec 24 23:59:59 2026 GMT
  host: routebase.dev
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 30 02:37:55 2026 GMT
  host: docs.routebase.dev
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 30 02:37:55 2026 GMT
  host: api.routebase.dev
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Routebase Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Routebase, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Routebase
provider_slug: routebase
slug: routebase-domain-security
source_filename: routebase-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: routebase.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 24 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.routebase.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 30 02:37:55 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\n- host: api.routebase.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 30 02:37:55 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\ndomains:\n- domain: routebase.dev\n  dnssec: true\n  caa:\n  - 0 iodef \"mailto:denny.riedl@routebase.dev\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issuewild \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/routebase/refs/heads/main/security/routebase-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- API lifecycle management
- API Design
- OpenAPI
- API Documentation
- API Testing
- API Mocking
- API Monitoring
- API Security
- MCP
- AI Agents
- Developer Tools
- CI/CD
- REST
- OAuth 2.1
- SCIM
- Streamable HTTP
---
