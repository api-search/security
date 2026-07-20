---
api_specs:
- filename: color-eligibility-openapi.yml
  format: yaml
  label: Color Eligibility List API
  slug: color-eligibility-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/color/refs/heads/main/openapi/color-eligibility-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  - 0 issuewild "amazon.com"
  - 0 issuewild "letsencrypt.org"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: color.com
  spf: true
hosts:
- cert_expires: Nov  2 23:59:59 2026 GMT
  host: www.color.com
  hsts: true
  hsts_max_age: 1800
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 17 03:26:47 2026 GMT
  host: docs.color.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 13 23:59:59 2027 GMT
  host: api.color.com
  hsts: true
  hsts_max_age: 3600
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Color Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Color, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Color
provider_slug: color
slug: color-domain-security
source_filename: color-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.color.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  2 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 1800\n- host: docs.color.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 17 03:26:47 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.color.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 13 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 3600\ndomains:\n- domain: color.com\n  dnssec: false\n  caa:\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/color/refs/heads/main/security/color-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Health
- Healthcare
- Genomics
- Oncology
- Cancer Care
- Preventive Health
- Eligibility
- Virtual Care
---
