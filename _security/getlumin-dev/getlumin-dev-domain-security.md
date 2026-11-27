---
api_specs:
- filename: getlumin-dev-openapi-generated.yml
  format: yaml
  label: Lumin API
  slug: getlumin-dev-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/getlumin-dev/openapi/_ae-authored/getlumin-dev-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: getlumin.dev
  spf: true
hosts:
- cert_expires: Feb  3 10:15:22 2027 GMT
  host: getlumin.dev
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Lumin Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Lumin, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Lumin
provider_slug: getlumin-dev
slug: getlumin-dev-domain-security
source_filename: getlumin-dev-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-09'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: getlumin.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  3 10:15:22 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: getlumin.dev\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/getlumin-dev/security/getlumin-dev-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Monitoring
- Docker
- DevOps
- Software-as-a-Service
- Small Teams
---
