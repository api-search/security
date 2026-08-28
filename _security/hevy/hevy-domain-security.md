---
api_specs:
- filename: hevy-public-api-openapi.json
  format: json
  label: Hevy Public API
  slug: hevy-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hevy/refs/heads/main/openapi/hevy-public-api-openapi.json
- filename: hevy-gpt-action-openapi.json
  format: json
  label: Hevy GPT Action API
  slug: hevy-gpt-action-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hevy/refs/heads/main/openapi/hevy-gpt-action-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: hevyapp.com
  spf: true
- caa: []
  dmarc: false
  dnssec: true
  domain: hevy.com
  spf: false
hosts:
- cert_expires: Oct 24 03:01:51 2026 GMT
  host: www.hevyapp.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  8 02:23:58 2026 GMT
  host: api.hevyapp.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 13 17:09:06 2026 GMT
  host: hevy.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Hevy Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Hevy, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Hevy
provider_slug: hevy
slug: hevy-domain-security
source_filename: hevy-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.hevyapp.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 24 03:01:51 2026 GMT\n  hsts: false\n- host: api.hevyapp.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 02:23:58 2026 GMT\n  hsts: false\n- host: hevy.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 13 17:09:06 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: hevyapp.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: hevy.com\n  dnssec: true\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hevy/refs/heads/main/security/hevy-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Fitness
- Health
- Workout Tracking
- Strength Training
- Consumer Apps
- Mobile
- Quantified Self
- Personal Training
- Health Data
---
