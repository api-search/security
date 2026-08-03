---
api_specs:
- filename: abnormal-client-api-openapi-original.yml
  format: yaml
  label: Abnormal Security Client API
  slug: client-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/abnormal/refs/heads/main/openapi/abnormal-client-api-openapi-original.yml
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issue "amazonaws.com"
  - 0 issue "digicert.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: abnormal.ai
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: swaggerhub.com
  spf: true
hosts:
- cert_expires: Nov  8 23:59:59 2026 GMT
  host: abnormal.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 14 23:59:59 2026 GMT
  host: app.swaggerhub.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  6 00:01:41 2026 GMT
  host: api.abnormalplatform.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Abnormal Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Abnormal AI, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Abnormal AI
provider_slug: abnormal
slug: abnormal-domain-security
source_filename: abnormal-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: abnormal.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  8 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: app.swaggerhub.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 14 23:59:59 2026 GMT\n  hsts: null\n- host: api.abnormalplatform.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 00:01:41 2026 GMT\n  hsts: null\ndomains:\n- domain: abnormal.ai\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"digicert.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: swaggerhub.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/abnormal/refs/heads/main/security/abnormal-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Security
- Email Security
- Cybersecurity
- Threat Intelligence
- Artificial Intelligence
- SOAR
- Identity
- Compliance
---
