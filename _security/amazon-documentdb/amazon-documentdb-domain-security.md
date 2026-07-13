---
api_specs:
- filename: amazon-documentdb-openapi.yml
  format: yaml
  label: Amazon DocumentDB API
  slug: amazon-documentdb-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-documentdb/refs/heads/main/openapi/amazon-documentdb-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: amazon.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: amazonaws.com
  spf: true
hosts:
- cert_expires: Oct 17 23:59:59 2026 GMT
  host: aws.amazon.com
  hsts: true
  hsts_max_age: 47304000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 14 23:59:59 2026 GMT
  host: rds.amazonaws.com
  hsts: true
  hsts_max_age: 47304000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Amazon Documentdb Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Amazon DocumentDB, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Amazon DocumentDB
provider_slug: amazon-documentdb
slug: amazon-documentdb-domain-security
source_filename: amazon-documentdb-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: aws.amazon.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 17 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 47304000\n- host: rds.amazonaws.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 47304000\ndomains:\n- domain: amazon.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: amazonaws.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amazon-documentdb/refs/heads/main/security/amazon-documentdb-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Amazon Web Services
- Database
- Document Database
- DocumentDB
- Managed Database
- MongoDB
- NoSQL
---
