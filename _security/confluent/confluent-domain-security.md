---
api_specs:
- filename: confluent-openapi.yml
  format: yaml
  label: Confluent
  slug: confluent
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/confluent/refs/heads/main/openapi/confluent-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: confluent.io
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: confluent.cloud
  spf: true
hosts:
- cert_expires: Sep 15 09:44:59 2026 GMT
  host: www.confluent.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  6 23:59:59 2026 GMT
  host: api.confluent.cloud
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Confluent Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Confluent, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Confluent
provider_slug: confluent
slug: confluent-domain-security
source_filename: confluent-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.confluent.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 09:44:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.confluent.cloud\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  6 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: confluent.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: confluent.cloud\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/confluent/refs/heads/main/security/confluent-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags: []
---
