---
api_specs:
- filename: hint-health-hint-health-api-openapi.yml
  format: yaml
  label: Hint Health API
  slug: hint-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hint-health/refs/heads/main/openapi/hint-health-hint-health-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "amazonaws.com"
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: hint.com
  spf: true
hosts:
- cert_expires: Oct  9 02:26:54 2026 GMT
  host: www.hint.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  4 06:17:01 2026 GMT
  host: developers.hint.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 25 08:02:25 2026 GMT
  host: api.hint.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Hint Health Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Hint Health, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Hint Health
provider_slug: hint-health
slug: hint-health-domain-security
source_filename: hint-health-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.hint.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 02:26:54 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developers.hint.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 06:17:01 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.hint.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 25 08:02:25 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: hint.com\n  dnssec: false\n  caa:\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hint-health/refs/heads/main/security/hint-health-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Direct Primary Care
- DPC
- Healthcare
- Membership Management
- Patient Enrollment
- Medical Billing
- EMR
- Health Plans
---
