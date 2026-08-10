---
api_specs:
- filename: access-token-management
  format: yaml
  label: GraphQL Hive Console GraphQL API
  slug: graphql-hive-console-graphql-api
  spec_type: OpenAPI
  url: https://the-guild.dev/graphql/hive/docs/graphql-api/access-token-management
description: ''
domains:
- caa:
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: the-guild.dev
  spf: true
hosts:
- cert_expires: Sep 27 10:42:35 2026 GMT
  host: the-guild.dev
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Envelop Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for The Guild, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: The Guild
provider_slug: the-guild-dev
slug: envelop-domain-security
source_filename: envelop-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: the-guild.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 27 10:42:35 2026 GMT\n  hsts: false\ndomains:\n- domain: the-guild.dev\n  dnssec: true\n  caa:\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/the-guild-dev/refs/heads/main/security/envelop-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- API Composition
- API Gateway
- API Observability
- Breaking Change Detection
- CI/CD
- Code Generation
- Developer Tools
- Execution
- Federation
- GitHub Actions
- GraphQL
- JavaScript
- Microservices
- Middleware
- Mocking
- Open Source
- Plugins
- REST
- SDKs
- Scalars
- Schema
- Schema Composition
- Schema Merging
- Schema Registry
- Schema Stitching
- Schema Transformation
- Schema Validation
- Server
- Subscriptions
- The Guild
- Type Merging
- Type Safety
- TypeScript
- gRPC
---
