---
api_specs:
- filename: apache-hbase-regions-api-openapi.yml
  format: yaml
  label: Apache HBase Regions API
  slug: apache-hbase-regions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apache-hbase/refs/heads/main/openapi/apache-hbase-regions-api-openapi.yml
- filename: apache-hbase-rows-api-openapi.yml
  format: yaml
  label: Apache HBase Rows API
  slug: apache-hbase-rows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apache-hbase/refs/heads/main/openapi/apache-hbase-rows-api-openapi.yml
- filename: apache-hbase-scans-api-openapi.yml
  format: yaml
  label: Apache HBase Scans API
  slug: apache-hbase-scans-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apache-hbase/refs/heads/main/openapi/apache-hbase-scans-api-openapi.yml
- filename: apache-hbase-tables-api-openapi.yml
  format: yaml
  label: Apache HBase Tables API
  slug: apache-hbase-tables-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apache-hbase/refs/heads/main/openapi/apache-hbase-tables-api-openapi.yml
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
hosts:
- cert_expires: Aug 24 23:33:10 2026 GMT
  host: hbase.apache.org
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Apache Hbase Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Apache HBase, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Apache HBase
provider_slug: apache-hbase
slug: apache-hbase-domain-security
source_filename: apache-hbase-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: hbase.apache.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 23:33:10 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: apache.org\n  dnssec: false\n  caa:\n  - 0 iodef \"mailto:root@apache.org\"\n  - 0 issue \"globalsign.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"sectigo.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/apache-hbase/refs/heads/main/security/apache-hbase-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Apache
- Big Data
- Bigtable
- Database
- Hadoop
- NoSQL
- Open-Source
- Wide Column
---
