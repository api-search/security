---
api_specs:
- filename: abortion-policy-api-openapi.yml
  format: yaml
  label: Abortion Policy API
  slug: abortion-policy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/abortion-policy-api/refs/heads/main/openapi/abortion-policy-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: abortionpolicyapi.com
  spf: true
hosts:
- cert_expires: Sep 20 12:15:18 2026 GMT
  host: www.abortionpolicyapi.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  5 23:10:12 2026 GMT
  host: api.abortionpolicyapi.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Abortion Policy Api Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Abortion Policy API, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Abortion Policy API
provider_slug: abortion-policy-api
slug: abortion-policy-api-domain-security
source_filename: abortion-policy-api-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.abortionpolicyapi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 12:15:18 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: api.abortionpolicyapi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  5 23:10:12 2026 GMT\n  hsts: null\ndomains:\n- domain: abortionpolicyapi.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/abortion-policy-api/refs/heads/main/security/abortion-policy-api-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Abortion
- Policies
- Healthcare
- Government
---
