---
api_specs:
- filename: apache-iotdb-openapi-generated.yml
  format: yaml
  label: Apache IoTDB API
  slug: apache-iotdb-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/apache-iotdb/openapi/_ae-authored/apache-iotdb-openapi-generated.yml
description: ''
domains:
- caa:
  - 0 issue "globalsign.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "sectigo.com"
  - 0 issue "ssl.com"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "ssl.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: apache.org
  spf: true
hosts:
- cert_expires: Dec 22 21:43:09 2026 GMT
  host: iotdb.apache.org
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Apache IoTDB Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Apache IoTDB, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Apache IoTDB
provider_slug: apache-iotdb
slug: apache-iotdb-domain-security
source_filename: apache-iotdb-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-15'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: iotdb.apache.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 22 21:43:09 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: apache.org\n  dnssec: false\n  caa:\n  - 0 issue \"globalsign.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"ssl.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/apache-iotdb/security/apache-iotdb-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Time Series
- IoT
- Database
- Open Source
- Apache
---
