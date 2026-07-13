---
api_specs:
- filename: calm-partner-api-openapi.yml
  format: yaml
  label: Calm Partner API
  slug: calm-partner-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/calm-com/refs/heads/main/openapi/calm-partner-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: calm.com
  spf: true
hosts:
- cert_expires: Jan 19 23:59:59 2027 GMT
  host: www.calm.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar 18 23:59:59 2027 GMT
  host: partner.calm.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 19 23:59:59 2027 GMT
  host: auth.calm.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Calm Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Calm, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Calm
provider_slug: calm-com
slug: calm-com-domain-security
source_filename: calm-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.calm.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 19 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: partner.calm.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 18 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: auth.calm.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan 19 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: calm.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/calm-com/refs/heads/main/security/calm-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Mindfulness
- Meditation
- Sleep
- Mental Health
- Wellness
- Digital Health
- Mobile App
- Consumer
- Employee Wellness
- Digital Therapeutics
- B2B
---
