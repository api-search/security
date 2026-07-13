---
api_specs:
- filename: thought-industries-openapi.yml
  format: yaml
  label: Thought Industries REST API
  slug: rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thought-industries/refs/heads/main/openapi/thought-industries-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: thoughtindustries.com
  spf: true
hosts:
- cert_expires: Sep 22 23:42:11 2026 GMT
  host: www.thoughtindustries.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 30 10:37:32 2026 GMT
  host: developer.thoughtindustries.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Thought Industries Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Thought Industries, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Thought Industries
provider_slug: thought-industries
slug: thought-industries-domain-security
source_filename: thought-industries-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.thoughtindustries.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 23:42:11 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: developer.thoughtindustries.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 30 10:37:32 2026 GMT\n  hsts: false\ndomains:\n- domain: thoughtindustries.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/thought-industries/refs/heads/main/security/thought-industries-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Education
- Learning
- LMS
- LXP
- E-Learning
- Training
---
