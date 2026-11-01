---
api_specs:
- filename: getfleek-app-openapi-generated.yml
  format: yaml
  label: getfleek-app API
  slug: getfleek-app-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/getfleek-app/openapi/_ae-authored/getfleek-app-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: getfleek.app
  spf: true
hosts:
- cert_expires: Jan 23 15:12:02 2027 GMT
  host: getfleek.app
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Getfleek App Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for getfleek-app, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: getfleek-app
provider_slug: getfleek-app
slug: getfleek-app-domain-security
source_filename: getfleek-app-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: getfleek.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 23 15:12:02 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: getfleek.app\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/getfleek-app/security/getfleek-app-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Subscription
- Rewards
- Fintech
- ConsumerApp
- Platform
---
