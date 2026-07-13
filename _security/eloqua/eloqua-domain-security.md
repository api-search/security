---
api_specs:
- filename: eloqua-rest-openapi.yml
  format: yaml
  label: Eloqua REST API
  slug: eloqua-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eloqua/refs/heads/main/openapi/eloqua-rest-openapi.yml
- filename: eloqua-bulk-openapi.yml
  format: yaml
  label: Eloqua Bulk API
  slug: eloqua-bulk-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eloqua/refs/heads/main/openapi/eloqua-bulk-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  - 0 issue "letsencrypt.org"
  - 0 issue "digicert.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: oracle.com
  spf: true
- caa:
  - 0 issuewild "www.digicert.com"
  - 0 issue "www.digicert.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: eloqua.com
  spf: true
hosts:
- cert_expires: Nov 15 23:59:59 2026 GMT
  host: docs.oracle.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  1 23:59:59 2026 GMT
  host: secure.p01.eloqua.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Eloqua Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Oracle Eloqua, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Oracle Eloqua
provider_slug: eloqua
slug: eloqua-domain-security
source_filename: eloqua-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docs.oracle.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 15 23:59:59 2026 GMT\n  hsts: false\n- host: secure.p01.eloqua.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: oracle.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"digicert.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: eloqua.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"www.digicert.com\"\n  - 0 issue \"www.digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/eloqua/refs/heads/main/security/eloqua-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- CRM
- Email Marketing
- Lead Management
- Marketing Automation
---
