---
api_specs:
- filename: mx_platform_api.yml
  format: yaml
  label: MX Platform API
  slug: mx-platform-api
  spec_type: OpenAPI
  url: https://github.com/mxenabled/openapi/blob/master/openapi/mx_platform_api.yml
description: ''
domains:
- caa:
  - 0 iodef "mailto:domains@mx.com"
  - 0 issue "awstrust.com"
  - 0 issue "amazon.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "digicert.com"
  - 0 issue "amazonaws.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: mx.com
  spf: true
hosts:
- cert_expires: Aug 31 23:59:59 2026 GMT
  host: www.mx.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 30 18:59:47 2026 GMT
  host: docs.mx.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 16 23:59:59 2027 GMT
  host: api.mx.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Mx Technologies Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for MX Technologies, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: MX Technologies
provider_slug: mx-technologies
slug: mx-technologies-domain-security
source_filename: mx-technologies-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.mx.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 31 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.mx.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 18:59:47 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.mx.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 16 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: mx.com\n  dnssec: false\n  caa:\n  - 0 iodef \"mailto:domains@mx.com\"\n  - 0 issue \"awstrust.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"amazonaws.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mx-technologies/refs/heads/main/security/mx-technologies-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Financial Data
- Account Aggregation
- Open Banking
- Data Connectivity
- Fintech
- Transaction Categorization
- Data Enhancement
- FDX
- Account Verification
- Personal Finance
---
