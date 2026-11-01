---
api_specs:
- filename: zigiwave-openapi-generated.yml
  format: yaml
  label: ZigiWave API
  slug: zigiwave-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/zigiwave/openapi/_ae-authored/zigiwave-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: zigiwave.com
  spf: true
hosts:
- cert_expires: Jan  3 10:03:45 2027 GMT
  host: zigiwave.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Zigiwave Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ZigiWave, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: ZigiWave
provider_slug: zigiwave
slug: zigiwave-domain-security
source_filename: zigiwave-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: zigiwave.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  3 10:03:45 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: zigiwave.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/zigiwave/security/zigiwave-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Integration
- Automation
- ITSM
- DevOps
- Software-as-a-Service
---
