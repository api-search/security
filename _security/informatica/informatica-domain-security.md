---
api_specs:
- filename: informatica-platform-rest-api-openapi.yml
  format: yaml
  label: Informatica Platform REST API
  slug: informatica
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/informatica/refs/heads/main/openapi/informatica-platform-rest-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: informatica.com
  spf: true
- caa:
  - 0 issuewild "identrust.com"
  - 0 issuewild "quovadisglobal.com"
  - 0 iodef "mailto:csoc@informatica.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: informaticacloud.com
  spf: true
hosts:
- cert_expires: Oct  2 15:07:36 2026 GMT
  host: developer.informatica.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  9 23:59:59 2026 GMT
  host: docs.informatica.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 13 12:36:43 2026 GMT
  host: dm-us.informaticacloud.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Informatica Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Informatica, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Informatica
provider_slug: informatica
slug: informatica-domain-security
source_filename: informatica-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developer.informatica.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 15:07:36 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.informatica.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: dm-us.informaticacloud.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 13 12:36:43 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: informatica.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: informaticacloud.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"identrust.com\"\n  - 0 issuewild \"quovadisglobal.com\"\n  - 0 iodef \"mailto:csoc@informatica.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/informatica/refs/heads/main/security/informatica-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Address Verification
- B2B Gateway
- Cloud Services
- Data Governance
- Data Integration
- Data Profiling
- Data Quality
- Enterprise Software
- ETL
- IDMC
- IICS
- Master Data Management
- Reference Data Management
---
