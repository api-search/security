---
api_specs:
- filename: feldera-openapi-original.json
  format: json
  label: Feldera API
  slug: feldera-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/feldera/refs/heads/main/openapi/feldera-openapi-original.json
description: ''
domains:
- caa:
  - 128 issue "letsencrypt.org"
  - 128 issue "pki.goog"
  - 128 issue "sectigo.com"
  - 128 issuewild ";"
  - 128 iodef "mailto:security@feldera.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: feldera.com
  spf: true
hosts:
- cert_expires: Sep 16 11:23:44 2026 GMT
  host: www.feldera.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Feldera Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Feldera, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Feldera
provider_slug: feldera
slug: feldera-domain-security
source_filename: feldera-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.feldera.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 11:23:44 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: feldera.com\n  dnssec: false\n  caa:\n  - 128 issue \"letsencrypt.org\"\n  - 128 issue \"pki.goog\"\n  - 128 issue \"sectigo.com\"\n  - 128 issuewild \";\"\n  - 128 iodef \"mailto:security@feldera.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/feldera/refs/heads/main/security/feldera-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Data Infrastructure
- Streaming
- SQL
- Incremental View Maintenance
- Real-Time Analytics
- Change Data Capture
- Materialized Views
- Data Pipelines
---
