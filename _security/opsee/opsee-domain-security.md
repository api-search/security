---
api_specs:
- filename: opsee-openapi-generated.yml
  format: yaml
  label: Opsee API
  slug: opsee-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/opsee/openapi/_ae-authored/opsee-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: opsee.io
  spf: true
hosts:
- cert_expires: Mar  7 23:59:59 2027 GMT
  host: opsee.io
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Opsee Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Opsee, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Opsee
provider_slug: opsee
slug: opsee-domain-security
source_filename: opsee-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: opsee.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar  7 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: opsee.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/opsee/security/opsee-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Manufacturing
- MES
- IndustrialIoT
- OpenSource
- DataAnalytics
---
