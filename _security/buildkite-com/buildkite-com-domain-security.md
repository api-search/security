---
api_specs:
- filename: buildkite-rest-api-openapi.yml
  format: yaml
  label: Buildkite REST API
  slug: buildkite-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/buildkite-com/refs/heads/main/openapi/buildkite-rest-api-openapi.yml
- filename: buildkite-agent-api-openapi.yml
  format: yaml
  label: Buildkite Agent API
  slug: buildkite-agent-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/buildkite-com/refs/heads/main/openapi/buildkite-agent-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "globalsign.com"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog"
  - 0 issuewild "sectigo.com"
  - 0 issue "amazonaws.com"
  - 0 issue "comodoca.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: buildkite.com
  spf: true
hosts:
- cert_expires: Jan  8 23:59:59 2027 GMT
  host: buildkite.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan  8 23:59:59 2027 GMT
  host: api.buildkite.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan  8 23:59:59 2027 GMT
  host: graphql.buildkite.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Buildkite Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Buildkite, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Buildkite
provider_slug: buildkite-com
slug: buildkite-com-domain-security
source_filename: buildkite-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: buildkite.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  8 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.buildkite.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  8 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: graphql.buildkite.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  8 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: buildkite.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"globalsign.com\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog\"\n  - 0 issuewild \"sectigo.com\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"comodoca.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/buildkite-com/refs/heads/main/security/buildkite-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- CI/CD
- Continuous Integration
- Continuous Delivery
- DevOps
- Pipelines
- Hybrid CI
- Build Automation
- Test Engine
- Package Registries
- Agents
- GraphQL
- REST
- MCP
- Webhooks
---
