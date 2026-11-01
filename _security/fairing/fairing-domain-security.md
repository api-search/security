---
api_specs:
- filename: fairing-questions-api-openapi.yml
  format: yaml
  label: Fairing Questions API
  slug: fairing-questions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fairing/openapi/fairing-questions-api-openapi.yml
- filename: fairing-responses-api-openapi.yml
  format: yaml
  label: Fairing Responses API
  slug: fairing-responses-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fairing/openapi/fairing-responses-api-openapi.yml
- filename: fairing-sources-api-openapi.yml
  format: yaml
  label: Fairing Sources API
  slug: fairing-sources-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fairing/openapi/fairing-sources-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: fairing.co
  spf: true
hosts:
- cert_expires: Jan  9 13:06:28 2027 GMT
  host: fairing.co
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Fairing Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Fairing, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Fairing
provider_slug: fairing
slug: fairing-domain-security
source_filename: fairing-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: fairing.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  9 13:06:28 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: fairing.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/fairing/security/fairing-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Post-Purchase
- Surveys
- Marketing
- Attribution
- Ecommerce
---
