---
api_specs:
- filename: datastax-devops-openapi.json
  format: json
  label: Astra DevOps API
  slug: astra-devops-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/datastax/refs/heads/main/openapi/datastax-devops-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: datastax.com
  spf: true
hosts:
- cert_expires: Aug 26 15:21:08 2026 GMT
  host: www.datastax.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb  7 23:59:59 2027 GMT
  host: docs.datastax.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 19 23:59:59 2027 GMT
  host: api.astra.datastax.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Datastax Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for DataStax, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: DataStax
provider_slug: datastax
slug: datastax-domain-security
source_filename: datastax-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.datastax.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 26 15:21:08 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.datastax.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  7 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.astra.datastax.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 19 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: datastax.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/datastax/refs/heads/main/security/datastax-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Enterprise
- Database
- Vector Database
- Cassandra
- Artificial Intelligence
- RAG
- Serverless
- Streaming
- Developer Tools
---
