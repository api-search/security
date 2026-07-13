---
api_specs:
- filename: spring-batch-51-openapi.yml
  format: yaml
  label: Spring Batch 5.1 Core API
  slug: spring-batch-51-core-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spring-batch-5-1/refs/heads/main/openapi/spring-batch-51-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "sectigo.com"
  - 0 issuewild "ssl.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: spring.io
  spf: true
hosts:
- cert_expires: Mar 27 23:59:59 2027 GMT
  host: docs.spring.io
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Spring Batch 5 1 Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Spring Batch 5.1, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Spring Batch 5.1
provider_slug: spring-batch-5-1
slug: spring-batch-5-1-domain-security
source_filename: spring-batch-5-1-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docs.spring.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 27 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: spring.io\n  dnssec: true\n  caa:\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"sectigo.com\"\n  - 0 issuewild \"ssl.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/spring-batch-5-1/refs/heads/main/security/spring-batch-5-1-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Batch Processing
- Data Processing
- Enterprise
- ETL
- Java
- Job Scheduling
- Spring Framework
---
