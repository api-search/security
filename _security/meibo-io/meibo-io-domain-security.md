---
api_specs:
- filename: meibo-io-entries-api-openapi.yml
  format: yaml
  label: meibo Entries API
  slug: meibo-io-entries-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/meibo-io/openapi/meibo-io-entries-api-openapi.yml
- filename: meibo-io-invites-api-openapi.yml
  format: yaml
  label: meibo Invites API
  slug: meibo-io-invites-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/meibo-io/openapi/meibo-io-invites-api-openapi.yml
- filename: meibo-io-moderation-api-openapi.yml
  format: yaml
  label: meibo Moderation API
  slug: meibo-io-moderation-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/meibo-io/openapi/meibo-io-moderation-api-openapi.yml
- filename: meibo-io-settings-api-openapi.yml
  format: yaml
  label: meibo Settings API
  slug: meibo-io-settings-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/meibo-io/openapi/meibo-io-settings-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: meibo.io
  spf: true
hosts:
- cert_expires: Apr 13 23:59:59 2027 GMT
  host: meibo.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: meibo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for meibo, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: meibo
provider_slug: meibo-io
slug: meibo-io-domain-security
source_filename: meibo-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: meibo.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Apr 13 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: meibo.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/meibo-io/security/meibo-io-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Education
- Directory
- Privacy
- Software-as-a-Service
- Schools
---
