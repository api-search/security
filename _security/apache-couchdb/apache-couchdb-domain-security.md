---
api_specs:
- filename: apache-couchdb-http-api-openapi.yaml
  format: yaml
  label: Apache CouchDB HTTP API
  slug: apache-couchdb-http-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apache-couchdb/refs/heads/main/openapi/apache-couchdb-http-api-openapi.yaml
description: ''
domains:
- caa:
  - 0 iodef "mailto:root@apache.org"
  - 0 issue "globalsign.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "sectigo.com"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: apache.org
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: couchdb.org
  spf: false
hosts:
- cert_expires: Aug 24 23:33:10 2026 GMT
  host: couchdb.apache.org
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  3 12:43:35 2026 GMT
  host: docs.couchdb.org
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Apache Couchdb Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Apache CouchDB, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Apache CouchDB
provider_slug: apache-couchdb
slug: apache-couchdb-domain-security
source_filename: apache-couchdb-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: couchdb.apache.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 23:33:10 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.couchdb.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 12:43:35 2026 GMT\n  hsts: false\ndomains:\n- domain: apache.org\n  dnssec: false\n  caa:\n  - 0 iodef \"mailto:root@apache.org\"\n  - 0 issue \"globalsign.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"sectigo.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: couchdb.org\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/apache-couchdb/refs/heads/main/security/apache-couchdb-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Apache
- Database
- Document Store
- JSON
- NoSQL
- Open Source
- Replication
- REST
---
