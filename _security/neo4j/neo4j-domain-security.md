---
api_specs:
- filename: neo4j-http-api-openapi.yml
  format: yaml
  label: Neo4j HTTP API
  slug: http-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/neo4j/refs/heads/main/openapi/neo4j-http-api-openapi.yml
- filename: neo4j-query-api-openapi.yml
  format: yaml
  label: Neo4j Query API
  slug: query-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/neo4j/refs/heads/main/openapi/neo4j-query-api-openapi.yml
- filename: neo4j-aura-api-openapi.yml
  format: yaml
  label: Neo4j Aura API
  slug: aura-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/neo4j/refs/heads/main/openapi/neo4j-aura-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "sectigo.com"
  - 0 issue "ssl.com"
  - 0 issue "starfieldtech.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: neo4j.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: neo4j.io
  spf: false
hosts:
- cert_expires: Sep 10 16:44:37 2026 GMT
  host: neo4j.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 21 08:03:04 2026 GMT
  host: api.neo4j.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Neo4J Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Neo4j, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Neo4j
provider_slug: neo4j
slug: neo4j-domain-security
source_filename: neo4j-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: neo4j.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 10 16:44:37 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.neo4j.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 21 08:03:04 2026 GMT\n  hsts: null\ndomains:\n- domain: neo4j.com\n  dnssec: true\n  caa:\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"ssl.com\"\n  - 0 issue \"starfieldtech.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: neo4j.io\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/neo4j/refs/heads/main/security/neo4j-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Graph Database
- Cypher
- Cloud
- GraphQL
- Drivers
- APIs
---
