---
api_specs:
- filename: deeplead-account-api-openapi.yml
  format: yaml
  label: Deeplead Account API
  slug: deeplead-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deeplead/refs/heads/main/openapi/deeplead-account-api-openapi.yml
- filename: deeplead-businesses-api-openapi.yml
  format: yaml
  label: Deeplead Businesses API
  slug: deeplead-businesses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deeplead/refs/heads/main/openapi/deeplead-businesses-api-openapi.yml
- filename: deeplead-contacts-api-openapi.yml
  format: yaml
  label: Deeplead Contacts API
  slug: deeplead-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deeplead/refs/heads/main/openapi/deeplead-contacts-api-openapi.yml
- filename: deeplead-deliverability-api-openapi.yml
  format: yaml
  label: Deeplead Deliverability API
  slug: deeplead-deliverability-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deeplead/refs/heads/main/openapi/deeplead-deliverability-api-openapi.yml
- filename: deeplead-organizations-api-openapi.yml
  format: yaml
  label: Deeplead Organizations API
  slug: deeplead-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deeplead/refs/heads/main/openapi/deeplead-organizations-api-openapi.yml
- filename: deeplead-persons-api-openapi.yml
  format: yaml
  label: Deeplead Persons API
  slug: deeplead-persons-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deeplead/refs/heads/main/openapi/deeplead-persons-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: deeplead.io
  spf: true
hosts:
- cert_expires: Nov 14 03:40:39 2026 GMT
  host: www.deeplead.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Deeplead Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Deeplead, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Deeplead
provider_slug: deeplead
slug: deeplead-domain-security
source_filename: deeplead-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.deeplead.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 14 03:40:39 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: deeplead.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/deeplead/refs/heads/main/security/deeplead-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Lead Generation
- Cold Email
- Artificial Intelligence
- Sales Automation
---
