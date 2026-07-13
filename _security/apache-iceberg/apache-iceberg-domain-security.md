---
api_specs:
- filename: apache-iceberg-rest-catalog-open-api.yaml
  format: yaml
  label: Apache Iceberg REST Catalog API
  slug: rest-catalog-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apache-iceberg/refs/heads/main/openapi/apache-iceberg-rest-catalog-open-api.yaml
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "sectigo.com"
  - 0 iodef "mailto:root@apache.org"
  - 0 issue "globalsign.com"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: apache.org
  spf: true
hosts:
- cert_expires: Aug 24 23:33:10 2026 GMT
  host: iceberg.apache.org
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 18 11:17:47 2026 GMT
  host: py.iceberg.apache.org
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Apache Iceberg Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Apache Iceberg, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Apache Iceberg
provider_slug: apache-iceberg
slug: apache-iceberg-domain-security
source_filename: apache-iceberg-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: iceberg.apache.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 23:33:10 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: py.iceberg.apache.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 11:17:47 2026 GMT\n  hsts: false\ndomains:\n- domain: apache.org\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"sectigo.com\"\n  - 0 iodef \"mailto:root@apache.org\"\n  - 0 issue \"globalsign.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/apache-iceberg/refs/heads/main/security/apache-iceberg-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- ACID
- Analytics
- Apache
- Data Lake
- Lakehouse
- Open Source
- Table Format
---
