---
api_specs:
- filename: openapi.yaml
  format: yaml
  label: Reflektive API
  slug: reflektive-api
  spec_type: OpenAPI
  url: https://docs.api.reflektive.com/
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: reflektive.com
  spf: true
hosts:
- cert_expires: Oct 19 23:59:59 2026 GMT
  host: www.reflektive.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
- cert_expires: Sep 18 18:45:49 2026 GMT
  host: docs.api.reflektive.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 19 23:59:59 2026 GMT
  host: api.reflektive.com
  hsts: true
  hsts_max_age: 31556952
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Reflektive Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Reflektive, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.2); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Reflektive
provider_slug: reflektive
slug: reflektive-domain-security
source_filename: reflektive-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.reflektive.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct 19 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.api.reflektive.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 18:45:49 2026 GMT\n  hsts: false\n- host: api.reflektive.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct 19 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31556952\ndomains:\n- domain: reflektive.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/reflektive/refs/heads/main/security/reflektive-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Performance Management
- HR
- Employee Feedback
- Goal Tracking
- Engagement Surveys
- Reviews
- People Analytics
- REST API
---
