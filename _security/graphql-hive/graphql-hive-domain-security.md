---
api_specs:
- filename: access-token-management
  format: yaml
  label: GraphQL Hive Console GraphQL API
  slug: graphql-hive-graphql-api
  spec_type: OpenAPI
  url: https://the-guild.dev/graphql/hive/docs/graphql-api/access-token-management
description: ''
domains:
- caa:
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: the-guild.dev
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: graphql-hive.com
  spf: true
hosts:
- cert_expires: Sep 27 10:42:35 2026 GMT
  host: the-guild.dev
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 18 14:18:03 2026 GMT
  host: api.graphql-hive.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Graphql Hive Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for GraphQL Hive, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: GraphQL Hive
provider_slug: graphql-hive
slug: graphql-hive-domain-security
source_filename: graphql-hive-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: the-guild.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 27 10:42:35 2026 GMT\n  hsts: false\n- host: api.graphql-hive.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 14:18:03 2026 GMT\n  hsts: null\ndomains:\n- domain: the-guild.dev\n  dnssec: true\n  caa:\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: graphql-hive.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/graphql-hive/refs/heads/main/security/graphql-hive-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- GraphQL
- Schema Registry
- API Observability
- Breaking Change Detection
- Federation
- Open Source
- Developer Tools
---
