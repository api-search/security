---
api_specs:
- filename: smarthr-openapi.yml
  format: yaml
  label: SmartHR Crews API
  slug: smarthr-crews-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smarthr/refs/heads/main/openapi/smarthr-openapi.yml
- filename: smarthr-openapi.yml
  format: yaml
  label: SmartHR Departments API
  slug: smarthr-departments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smarthr/refs/heads/main/openapi/smarthr-openapi.yml
- filename: smarthr-openapi.yml
  format: yaml
  label: SmartHR Employment Types API
  slug: smarthr-employment-types-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smarthr/refs/heads/main/openapi/smarthr-openapi.yml
- filename: smarthr-openapi.yml
  format: yaml
  label: SmartHR Custom Field Templates API
  slug: smarthr-custom-field-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smarthr/refs/heads/main/openapi/smarthr-openapi.yml
- filename: smarthr-openapi.yml
  format: yaml
  label: SmartHR Business Establishments API
  slug: smarthr-business-establishments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smarthr/refs/heads/main/openapi/smarthr-openapi.yml
- filename: smarthr-openapi.yml
  format: yaml
  label: SmartHR Webhooks API
  slug: smarthr-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smarthr/refs/heads/main/openapi/smarthr-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: smarthr.jp
  spf: true
  spf_policy: -all
- caa:
  - 0 issue "globalsign.com"
  - 0 issue "letsencrypt.org"
  dmarc: false
  dnssec: false
  domain: developer.smarthr.jp
  note: developer.smarthr.jp is served via Vercel (CNAME cname.vercel-dns.com).
  spf: false
hosts:
- cert_expires: Oct  7 08:23:24 2026 GMT
  host: smarthr.jp
  hsts: true
  hsts_max_age: 0
  hsts_note: HSTS header present but max-age=0 (effectively not enforcing).
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 24 20:21:34 2026 GMT
  host: developer.smarthr.jp
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Smarthr Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SmartHR, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: SmartHR
provider_slug: smarthr
slug: smarthr-domain-security
source_filename: smarthr-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + documentation hosts\nhosts:\n- host: smarthr.jp\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 08:23:24 2026 GMT\n  hsts: true\n  hsts_max_age: 0\n  hsts_note: HSTS header present but max-age=0 (effectively not enforcing).\n- host: developer.smarthr.jp\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 20:21:34 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: smarthr.jp\n  dnssec: false\n  caa: []\n  spf: true\n  spf_policy: '-all'\n  dmarc: true\n  dmarc_policy: reject\n- domain: developer.smarthr.jp\n  dnssec: false\n  caa:\n  - '0 issue \"globalsign.com\"'\n  - '0 issue \"letsencrypt.org\"'\n  spf: false\n  dmarc: false\n  note: developer.smarthr.jp is served via Vercel (CNAME cname.vercel-dns.com).\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/smarthr/refs/heads/main/security/smarthr-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- HR
- Human Resources
- HRIS
- Labor Management
- Payroll
- Japan
- Employees
- Personnel
- Onboarding
- SaaS
---
