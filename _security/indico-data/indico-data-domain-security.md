---
api_specs:
- filename: indico-data-openapi.yml
  format: yaml
  label: Indico REST API
  slug: indico-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/indico-data/refs/heads/main/openapi/indico-data-openapi.yml
description: ''
domains:
- caa:
  - 128 issue "sectigo.com"
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: indicodata.ai
  spf: true
- caa:
  - 0 issue "sectigo.com"
  - 128 issuewild "sectigo.com"
  - 0 issue "amazon.com"
  - 0 issue "amazonaws.com"
  - 0 issue "amazontrust.com"
  - 0 issue "awstrust.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: indico.io
  spf: true
hosts:
- cert_expires: Aug 23 12:24:01 2026 GMT
  host: indicodata.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  1 18:16:50 2026 GMT
  host: developer.indicodata.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- host: app.indico.io
  https: false
kind: domain-security
layout: security
method: probed
name: Indico Data Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Indico Data, probed live across 3 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Indico Data
provider_slug: indico-data
slug: indico-data-domain-security
source_filename: indico-data-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: indicodata.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 23 12:24:01 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: developer.indicodata.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  1 18:16:50 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: app.indico.io\n  https: false\ndomains:\n- domain: indicodata.ai\n  dnssec: false\n  caa:\n  - 128 issue \"sectigo.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: indico.io\n  dnssec: false\n  caa:\n  - 0 issue \"sectigo.com\"\n  - 128 issuewild \"sectigo.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"awstrust.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/indico-data/refs/heads/main/security/indico-data-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Intelligent Document Processing
- Intelligent Process Automation
- Document AI
- Machine Learning
- Unstructured Data
- Data Extraction
- Insurance
---
