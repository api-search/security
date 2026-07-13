---
api_specs:
- filename: leapsome-content-api-openapi.yml
  format: yaml
  label: Leapsome Content API
  slug: leapsome-content-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leapsome/refs/heads/main/openapi/leapsome-content-api-openapi.yml
- filename: leapsome-scim-api-openapi.yml
  format: yaml
  label: Leapsome SCIM API
  slug: leapsome-scim-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leapsome/refs/heads/main/openapi/leapsome-scim-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: leapsome.com
  spf: true
hosts:
- cert_expires: Feb  2 23:59:59 2027 GMT
  host: www.leapsome.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 20 23:41:15 2026 GMT
  host: help.leapsome.com
  hsts: true
  hsts_max_age: 259200
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 15 23:59:59 2026 GMT
  host: api.leapsome.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Leapsome Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Leapsome, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Leapsome
provider_slug: leapsome
slug: leapsome-domain-security
source_filename: leapsome-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.leapsome.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  2 23:59:59 2027 GMT\n  hsts: false\n- host: help.leapsome.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 23:41:15 2026 GMT\n  hsts: true\n  hsts_max_age: 259200\n- host: api.leapsome.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 15 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: leapsome.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/leapsome/refs/heads/main/security/leapsome-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- People Enablement
- Performance Management
- OKRs
- Goals
- Engagement Surveys
- HRIS
- SCIM
- Employee Development
- 1:1 Meetings
- Learning
---
