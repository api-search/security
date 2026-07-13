---
api_specs:
- filename: personio-auth-api.yaml
  format: yaml
  label: Personio Public API v1
  slug: public-api-v1
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/personio/api-docs/master/personio-auth-api.yaml
- filename: personio-openapi.yml
  format: yaml
  label: Personio Public API v2
  slug: public-api-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/personio/refs/heads/main/openapi/personio-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: personio.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: personio.de
  spf: true
hosts:
- cert_expires: Aug 27 11:23:50 2026 GMT
  host: www.personio.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 20 22:12:07 2026 GMT
  host: developer.personio.de
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 16 23:59:59 2026 GMT
  host: api.personio.de
  hsts: true
  hsts_max_age: 31540000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Personio Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Personio, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Personio
provider_slug: personio
slug: personio-domain-security
source_filename: personio-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.personio.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 27 11:23:50 2026 GMT\n  hsts: null\n- host: developer.personio.de\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 22:12:07 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.personio.de\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31540000\ndomains:\n- domain: personio.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: personio.de\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/personio/refs/heads/main/security/personio-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Human Resources
- HRIS
- Recruiting
- Applicant Tracking
- Absence Management
- Time Tracking
- Europe HR
---
