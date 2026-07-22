---
api_specs:
- filename: wellhub-integrations-openapi-original.json
  format: json
  label: Wellhub Integrations API
  slug: wellhub-integrations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wellhub/refs/heads/main/openapi/wellhub-integrations-openapi-original.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: wellhub.com
  spf: true
hosts:
- cert_expires: Jan 23 23:59:59 2027 GMT
  host: wellhub.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar  3 23:59:59 2027 GMT
  host: api.clients.wellhub.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Wellhub Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Wellhub, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Wellhub
provider_slug: wellhub
slug: wellhub-domain-security
source_filename: wellhub-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: wellhub.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 23 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.clients.wellhub.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar  3 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: wellhub.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wellhub/refs/heads/main/security/wellhub-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Health
- Wellbeing
- Corporate Benefits
- Fitness
- HR
- Eligibility
- Employee Benefits
---
