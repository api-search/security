---
api_specs:
- filename: spark-hire-openapi.yml
  format: yaml
  label: Spark Hire Interviews API
  slug: spark-hire-interviews-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spark-hire/refs/heads/main/openapi/spark-hire-openapi.yml
- filename: spark-hire-openapi.yml
  format: yaml
  label: Spark Hire Interview Questions API
  slug: spark-hire-interview-questions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spark-hire/refs/heads/main/openapi/spark-hire-openapi.yml
- filename: spark-hire-openapi.yml
  format: yaml
  label: Spark Hire Jobs API
  slug: spark-hire-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spark-hire/refs/heads/main/openapi/spark-hire-openapi.yml
- filename: spark-hire-openapi.yml
  format: yaml
  label: Spark Hire Users API
  slug: spark-hire-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spark-hire/refs/heads/main/openapi/spark-hire-openapi.yml
- filename: spark-hire-openapi.yml
  format: yaml
  label: Spark Hire Webhooks API
  slug: spark-hire-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spark-hire/refs/heads/main/openapi/spark-hire-openapi.yml
- filename: spark-hire-openapi.yml
  format: yaml
  label: Spark Hire Account and Plan API
  slug: spark-hire-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spark-hire/refs/heads/main/openapi/spark-hire-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issue "amazon.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issuewild "amazon.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: sparkhire.com
  spf: true
hosts:
- cert_expires: Aug 20 01:12:38 2026 GMT
  host: www.sparkhire.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb  1 23:59:59 2027 GMT
  host: docs.sparkhire.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb  1 23:59:59 2027 GMT
  host: api.sparkhire.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Spark Hire Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Spark Hire, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Spark Hire
provider_slug: spark-hire
slug: spark-hire-domain-security
source_filename: spark-hire-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.sparkhire.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 20 01:12:38 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.sparkhire.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  1 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.sparkhire.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  1 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: sparkhire.com\n  dnssec: true\n  caa:\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issuewild \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/spark-hire/refs/heads/main/security/spark-hire-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Video Interviewing
- Recruiting
- Hiring
- HR Tech
- Talent Assessment
- ATS
---
