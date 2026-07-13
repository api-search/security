---
api_specs:
- filename: mx-platform-openapi.yml
  format: yaml
  label: MX Platform API
  slug: mx-platform
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mx-platform/main/openapi/mx-platform-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "amazon.com"
  - 0 issue "amazonaws.com"
  - 0 issue "digicert.com"
  - 0 issue "amazontrust.com"
  - 0 iodef "mailto:domains@mx.com"
  - 0 issue "certainly.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: mx.com
  spf: true
hosts:
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
name: Mx Platform Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for MX Platform, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: MX Platform
provider_slug: mx-platform
slug: mx-platform-domain-security
source_filename: mx-platform-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docs.mx.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 18:59:47 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.mx.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 16 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: mx.com\n  dnssec: false\n  caa:\n  - 0 issue \"amazon.com\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"amazontrust.com\"\n  - 0 iodef \"mailto:domains@mx.com\"\n  - 0 issue \"certainly.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mx-platform/refs/heads/main/security/mx-platform-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Aggregation
- Banking
- Financial
- Financial Data
---
