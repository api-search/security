---
api_specs:
- filename: oracle-goldengate-rest-api-openapi.yml
  format: yaml
  label: Oracle GoldenGate REST API
  slug: oracle-goldengate-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oracle-goldengate/refs/heads/main/openapi/oracle-goldengate-rest-api-openapi.yml
- filename: oracle-goldengate-big-data-rest-api-openapi.yml
  format: yaml
  label: Oracle GoldenGate for Big Data REST API
  slug: oracle-goldengate-for-big-data-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oracle-goldengate/refs/heads/main/openapi/oracle-goldengate-big-data-rest-api-openapi.yml
- filename: oracle-goldengate-veridata-rest-api-openapi.yml
  format: yaml
  label: Oracle GoldenGate Veridata REST API
  slug: oracle-goldengate-veridata-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oracle-goldengate/refs/heads/main/openapi/oracle-goldengate-veridata-rest-api-openapi.yml
- filename: oracle-goldengate-cloud-service-api-openapi.yml
  format: yaml
  label: Oracle GoldenGate Cloud Service API
  slug: oracle-goldengate-cloud-service-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oracle-goldengate/refs/heads/main/openapi/oracle-goldengate-cloud-service-api-openapi.yml
- filename: oracle-goldengate-stream-analytics-rest-api-openapi.yml
  format: yaml
  label: Oracle GoldenGate Stream Analytics REST API
  slug: oracle-goldengate-stream-analytics-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oracle-goldengate/refs/heads/main/openapi/oracle-goldengate-stream-analytics-rest-api-openapi.yml
- filename: oracle-goldengate-data-streams-rest-api-openapi.yml
  format: yaml
  label: Oracle GoldenGate Data Streams REST API
  slug: oracle-goldengate-data-streams-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oracle-goldengate/refs/heads/main/openapi/oracle-goldengate-data-streams-rest-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "digicert.com"
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: oracle.com
  spf: true
hosts:
- cert_expires: Feb  7 23:59:59 2027 GMT
  host: www.oracle.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 15 23:59:59 2026 GMT
  host: docs.oracle.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Oracle Goldengate Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Oracle GoldenGate, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Oracle GoldenGate
provider_slug: oracle-goldengate
slug: oracle-goldengate-domain-security
source_filename: oracle-goldengate-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.oracle.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  7 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.oracle.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 15 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: oracle.com\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/oracle-goldengate/refs/heads/main/security/oracle-goldengate-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- CDC
- Data Integration
- Data Synchronization
- Database
- Enterprise
- Real-Time Replication
---
