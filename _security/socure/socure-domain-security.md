---
api_specs:
- filename: socure-alerts-api-openapi.yml
  format: yaml
  label: socure Alerts API
  slug: socure-alerts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/socure/refs/heads/main/openapi/socure-alerts-api-openapi.yml
- filename: socure-id-api-openapi.yml
  format: yaml
  label: socure ID+ API
  slug: socure-id-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/socure/refs/heads/main/openapi/socure-id-api-openapi.yml
- filename: socure-monitoring-api-openapi.yml
  format: yaml
  label: socure Monitoring API
  slug: socure-monitoring-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/socure/refs/heads/main/openapi/socure-monitoring-api-openapi.yml
- filename: socure-transactions-api-openapi.yml
  format: yaml
  label: socure Transactions API
  slug: socure-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/socure/refs/heads/main/openapi/socure-transactions-api-openapi.yml
- filename: socure-uploads-api-openapi.yml
  format: yaml
  label: socure Uploads API
  slug: socure-uploads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/socure/refs/heads/main/openapi/socure-uploads-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "amazon.com"
  - 0 issue "amazon.com"
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: socure.com
  spf: true
hosts:
- cert_expires: Aug 20 05:55:26 2026 GMT
  host: www.socure.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 28 23:59:59 2026 GMT
  host: developer.socure.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 29 05:44:40 2026 GMT
  host: help.socure.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Socure Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for socure, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: socure
provider_slug: socure
slug: socure-domain-security
source_filename: socure-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.socure.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 20 05:55:26 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: developer.socure.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 28 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: help.socure.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 05:44:40 2026 GMT\n  hsts: null\ndomains:\n- domain: socure.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"amazon.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/socure/refs/heads/main/security/socure-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags: []
---
