---
api_specs:
- filename: openapi.json
  format: json
  label: MongoDB Atlas Administration API v2
  slug: administration-api-v2
  spec_type: OpenAPI
  url: https://mongodb-mms-prod-build-server.s3.amazonaws.com/openapi/openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: mongodb.com
  spf: true
hosts:
- cert_expires: Feb  4 23:59:59 2027 GMT
  host: www.mongodb.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 11 15:01:52 2026 GMT
  host: cloud.mongodb.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Mongodb Atlas Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for MongoDB Atlas, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: MongoDB Atlas
provider_slug: mongodb-atlas
slug: mongodb-atlas-domain-security
source_filename: mongodb-atlas-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.mongodb.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  4 23:59:59 2027 GMT\n  hsts: false\n- host: cloud.mongodb.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 11 15:01:52 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: mongodb.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mongodb-atlas/refs/heads/main/security/mongodb-atlas-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Database
- Document Database
- NoSQL
- MongoDB
- Cloud Database
- DBaaS
- Vector Search
- Atlas
---
