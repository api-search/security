---
api_specs:
- filename: bloomberg-data-license-api.yml
  format: yaml
  label: Bloomberg Data License API
  slug: bloomberg-data-license-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bloomberg-aim/refs/heads/main/openapi/bloomberg-data-license-api.yml
- filename: bloomberg-emsx-api.yml
  format: yaml
  label: Bloomberg EMSX API
  slug: bloomberg-emsx-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bloomberg-aim/refs/heads/main/openapi/bloomberg-emsx-api.yml
- filename: bloomberg-http-api.yml
  format: yaml
  label: Bloomberg HTTP API
  slug: bloomberg-http-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bloomberg-aim/refs/heads/main/openapi/bloomberg-http-api.yml
description: ''
domains:
- caa:
  - 0 issuewild "digicert.com"
  - 0 iodef "mailto:reportvuln@bloomberg.net"
  - 0 issue "amazon.com"
  - 0 issue "digicert.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: bloomberg.com
  spf: true
hosts:
- cert_expires: Mar 13 23:59:59 2027 GMT
  host: developer.bloomberg.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 14 23:59:59 2027 GMT
  host: www.bloomberg.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar 21 23:59:59 2027 GMT
  host: api.bloomberg.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Bloomberg Aim Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bloomberg AIM, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Bloomberg AIM
provider_slug: bloomberg-aim
slug: bloomberg-aim-domain-security
source_filename: bloomberg-aim-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developer.bloomberg.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 13 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: www.bloomberg.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 14 23:59:59 2027 GMT\n  hsts: null\n- host: api.bloomberg.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 21 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: bloomberg.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"digicert.com\"\n  - 0 iodef \"mailto:reportvuln@bloomberg.net\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"digicert.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bloomberg-aim/refs/heads/main/security/bloomberg-aim-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Financial Data
- Market Data
- Order Management
- Portfolio Management
- Trading
---
