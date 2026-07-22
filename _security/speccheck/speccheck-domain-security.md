---
api_specs:
- filename: speccheck-openapi.yml
  format: yaml
  label: SpecCheck API
  slug: speccheck-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/speccheck/refs/heads/main/openapi/speccheck-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: speccheckrx.com
  spf: true
hosts:
- cert_expires: Sep 29 05:17:46 2026 GMT
  host: speccheckrx.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 31 23:59:59 2027 GMT
  host: api.speccheckrx.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan  3 23:59:59 2027 GMT
  host: api-staging.speccheckrx.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Speccheck Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SpecCheck, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: SpecCheck
provider_slug: speccheck
slug: speccheck-domain-security
source_filename: speccheck-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: speccheckrx.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 05:17:46 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.speccheckrx.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 31 23:59:59 2027 GMT\n  hsts: null\n- host: api-staging.speccheckrx.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  3 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: speccheckrx.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/speccheck/refs/heads/main/security/speccheck-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Enterprise Saas
- Optical
- Eyewear
- Eyecare
- Optical Labs
- Prescriptions
- Ordering
- Healthcare
---
