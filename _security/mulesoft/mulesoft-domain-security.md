---
api_specs:
- filename: mulesoft-anypoint-platform-openapi.yml
  format: yaml
  label: MuleSoft Anypoint Platform Management API
  slug: mulesoft-anypoint-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mulesoft/refs/heads/main/openapi/mulesoft-anypoint-platform-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: mulesoft.com
  spf: true
hosts:
- cert_expires: Jan 19 23:59:59 2027 GMT
  host: www.mulesoft.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.2
- cert_expires: Jan 31 23:59:59 2027 GMT
  host: docs.mulesoft.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 23 23:59:59 2026 GMT
  host: anypoint.mulesoft.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Mulesoft Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for MuleSoft, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.2); 3 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: MuleSoft
provider_slug: mulesoft
slug: mulesoft-domain-security
source_filename: mulesoft-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.mulesoft.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan 19 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.mulesoft.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 31 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: anypoint.mulesoft.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 23 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: mulesoft.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mulesoft/refs/heads/main/security/mulesoft-domain-security.yml
summary_line: TLSv1.2 · HSTS · DNSSEC · DMARC
tags:
- API Gateway
- API Management
- Enterprise
- Integration
---
