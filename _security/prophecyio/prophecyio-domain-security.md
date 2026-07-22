---
api_specs:
- filename: prophecyio-connections-openapi.json
  format: json
  label: Prophecy API
  slug: prophecy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prophecyio/refs/heads/main/openapi/prophecyio-connections-openapi.json
description: ''
domains:
- caa:
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog"
  - 0 iodef "mailto:security@prophecy.io"
  - 0 issue "amazon.com"
  - 0 issue "amazonaws.com"
  - 0 issue "amazontrust.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: prophecy.io
  spf: true
- caa:
  - 0 issue "awstrust.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issuewild "amazon.com"
  - 0 issuewild "amazonaws.com"
  - 0 issuewild "amazontrust.com"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: prophecy.ai
  spf: true
hosts:
- cert_expires: Sep 29 16:43:38 2026 GMT
  host: www.prophecy.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  2 21:20:43 2026 GMT
  host: docs.prophecy.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  3 23:59:59 2026 GMT
  host: app.prophecy.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Prophecyio Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Prophecy.io, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Prophecy.io
provider_slug: prophecyio
slug: prophecyio-domain-security
source_filename: prophecyio-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.prophecy.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 16:43:38 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.prophecy.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  2 21:20:43 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: app.prophecy.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  3 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: prophecy.io\n  dnssec: false\n  caa:\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog\"\n  - 0 iodef \"mailto:security@prophecy.io\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"amazontrust.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: prophecy.ai\n  dnssec: false\n  caa:\n  - 0 issue \"awstrust.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"\
  pki.goog\"\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"amazonaws.com\"\n  - 0 issuewild \"amazontrust.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/prophecyio/refs/heads/main/security/prophecyio-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Data Engineering
- Data Pipelines
- ETL
- Apache Spark
- Databricks
- Snowflake
- Low-Code
- Analytics
- AI
- Data Transformation
---
