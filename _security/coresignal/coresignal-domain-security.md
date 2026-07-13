---
api_specs:
- filename: coresignal-multi-source-company-api-openapi.yml
  format: yaml
  label: Coresignal Multi-source Company API
  slug: multi-source-company-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coresignal/refs/heads/main/openapi/coresignal-multi-source-company-api-openapi.yml
- filename: coresignal-multi-source-employee-api-openapi.yml
  format: yaml
  label: Coresignal Multi-source Employee API
  slug: multi-source-employee-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coresignal/refs/heads/main/openapi/coresignal-multi-source-employee-api-openapi.yml
- filename: coresignal-multi-source-jobs-api-openapi.yml
  format: yaml
  label: Coresignal Multi-source Jobs API
  slug: multi-source-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coresignal/refs/heads/main/openapi/coresignal-multi-source-jobs-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: coresignal.com
  spf: true
hosts:
- cert_expires: Aug 12 05:46:12 2026 GMT
  host: coresignal.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 14 22:44:53 2026 GMT
  host: docs.coresignal.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 27 16:46:54 2026 GMT
  host: api.coresignal.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Coresignal Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Coresignal, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Coresignal
provider_slug: coresignal
slug: coresignal-domain-security
source_filename: coresignal-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: coresignal.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 12 05:46:12 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.coresignal.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 14 22:44:53 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.coresignal.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 27 16:46:54 2026 GMT\n  hsts: null\ndomains:\n- domain: coresignal.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/coresignal/refs/heads/main/security/coresignal-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Agentic Search
- B2B Data
- Companies
- Company Data
- Data as a Service
- Elasticsearch
- Employee Data
- Employees
- Enrichment
- Firmographics
- Job Postings
- Jobs
- Lead Generation
- People Data
- Sales Intelligence
- Talent Intelligence
- Web Data
---
