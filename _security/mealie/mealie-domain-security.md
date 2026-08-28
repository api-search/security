---
api_specs:
- filename: mealie-openapi.json
  format: json
  label: Mealie API
  slug: mealie-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mealie/refs/heads/main/openapi/mealie-openapi.json
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: mealie.io
  spf: false
hosts:
- cert_expires: Oct 18 23:00:06 2026 GMT
  host: mealie.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 18 23:00:06 2026 GMT
  host: docs.mealie.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 22 11:16:30 2026 GMT
  host: demo.mealie.io
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Mealie Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Mealie, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Mealie
provider_slug: mealie
slug: mealie-domain-security
source_filename: mealie-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: mealie.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 18 23:00:06 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.mealie.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 18 23:00:06 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: demo.mealie.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 22 11:16:30 2026 GMT\n  hsts: false\ndomains:\n- domain: mealie.io\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mealie/refs/heads/main/security/mealie-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Recipes
- Food
- Meal Planning
- Shopping Lists
- Self-Hosted
- Open Source
- Household
- Nutrition
- Home Automation
---
