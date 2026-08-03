---
api_specs:
- filename: arangodb-core-openapi-original.json
  format: json
  label: ArangoDB Core API
  slug: arangodb-core-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/arangodb/refs/heads/main/openapi/arangodb-core-openapi-original.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: arango.ai
  spf: true
- caa:
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "sectigo.com"
  - 0 issuewild "ssl.com"
  - 0 issue "comodoca.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: arangodb.com
  spf: true
hosts:
- cert_expires: Sep 24 18:02:10 2026 GMT
  host: arango.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 31 11:46:46 2026 GMT
  host: docs.arango.ai
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  4 12:15:11 2026 GMT
  host: api.cloud.arangodb.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Arangodb Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ArangoDB, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: ArangoDB
provider_slug: arangodb
slug: arangodb-domain-security
source_filename: arangodb-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: arango.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 18:02:10 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.arango.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 31 11:46:46 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\n- host: api.cloud.arangodb.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 12:15:11 2026 GMT\n  hsts: null\ndomains:\n- domain: arango.ai\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: arangodb.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"sectigo.com\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"comodoca.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/arangodb/refs/heads/main/security/arangodb-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Database
- Graph Database
- Multi-Model Database
- NoSQL
- Vector Search
- Knowledge Graph
- Developer Tools
- Cloud Infrastructure
- Artificial Intelligence
---
