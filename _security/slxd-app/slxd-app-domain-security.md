---
api_specs:
- filename: slxd-app-openapi-generated.yml
  format: yaml
  label: slxd-app API
  slug: slxd-app-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/slxd-app/openapi/_ae-authored/slxd-app-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: slxd.app
  spf: true
hosts:
- cert_expires: Jan 14 16:14:24 2027 GMT
  host: slxd.app
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Slxd App Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for slxd-app, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: slxd-app
provider_slug: slxd-app
slug: slxd-app-domain-security
source_filename: slxd-app-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: slxd.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 14 16:14:24 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: slxd.app\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/slxd-app/security/slxd-app-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Learning
- Education
- SaaS
- Platform
- Collaboration
---
