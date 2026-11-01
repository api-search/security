---
api_specs:
- filename: stract-api-my-user-api-openapi.yml
  format: yaml
  label: Stract API My User API
  slug: stract-api-my-user-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/stract-api/openapi/stract-api-my-user-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: stract-api.com
  spf: true
hosts:
- cert_expires: Feb 25 23:59:59 2027 GMT
  host: stract-api.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Stract Api Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Stract API, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Stract API
provider_slug: stract-api
slug: stract-api-domain-security
source_filename: stract-api-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: stract-api.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 25 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: stract-api.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/stract-api/security/stract-api-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- AI
- Document-Processing
- Data-Extraction
- SaaS
---
