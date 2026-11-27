---
api_specs:
- filename: postbye-com-api-openapi.json
  format: json
  label: Postbye API API
  slug: postbye-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/postbye-com/openapi/_original/postbye-com-api-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: postbye.com
  spf: true
hosts:
- cert_expires: Jan 24 17:45:09 2027 GMT
  host: postbye.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Postbye Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Postbye, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Postbye
provider_slug: postbye-com
slug: postbye-com-domain-security
source_filename: postbye-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-14'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: postbye.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 24 17:45:09 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: postbye.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/postbye-com/security/postbye-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Subscription cancellation
- Certified Mail
- Consumer Services
---
