---
api_specs:
- filename: mongodb-atlas-openapi.yaml
  format: yaml
  label: MongoDB Atlas Administration API
  slug: mongodb-atlas-administration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mongodb/refs/heads/main/openapi/mongodb-atlas-openapi.yaml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: mongodb.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: mongodb-api.com
  spf: false
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
- cert_expires: Aug 11 15:02:10 2026 GMT
  host: data.mongodb-api.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Mongodb Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for MongoDB, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: MongoDB
provider_slug: mongodb
slug: mongodb-domain-security
source_filename: mongodb-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.mongodb.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  4 23:59:59 2027 GMT\n  hsts: false\n- host: cloud.mongodb.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 11 15:01:52 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: data.mongodb-api.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 11 15:02:10 2026 GMT\n  hsts: null\ndomains:\n- domain: mongodb.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: mongodb-api.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mongodb/refs/heads/main/security/mongodb-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Cloud Database
- Database
- Document Database
- NoSQL
---
