---
api_specs:
- filename: comeet-careers-api-openapi.yml
  format: yaml
  label: Comeet Careers API
  slug: comeet-careers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/comeet/refs/heads/main/openapi/comeet-careers-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: comeet.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: comeet.co
  spf: true
hosts:
- cert_expires: Aug 24 23:33:42 2026 GMT
  host: www.comeet.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  2 20:08:12 2026 GMT
  host: developers.comeet.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 24 23:33:42 2026 GMT
  host: www.comeet.co
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Comeet Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Comeet, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Comeet
provider_slug: comeet
slug: comeet-domain-security
source_filename: comeet-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.comeet.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 23:33:42 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developers.comeet.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 20:08:12 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: www.comeet.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 23:33:42 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: comeet.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: comeet.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/comeet/refs/heads/main/security/comeet-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- ATS
- Candidates
- Careers
- Interviews
- Jobs
- Recruiting
- Talent Acquisition
---
