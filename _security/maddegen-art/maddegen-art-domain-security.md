---
api_specs:
- filename: maddegen-art-pump-cortex-api-openapi.yml
  format: yaml
  label: maddegen-art Pump Cortex API
  slug: maddegen-art-pump-cortex-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/maddegen-art/openapi/maddegen-art-pump-cortex-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: maddegen.art
  spf: true
hosts:
- cert_expires: Dec 19 12:53:03 2026 GMT
  host: maddegen.art
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Maddegen Art Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for maddegen-art, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: maddegen-art
provider_slug: maddegen-art
slug: maddegen-art-domain-security
source_filename: maddegen-art-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: maddegen.art\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 19 12:53:03 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: maddegen.art\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/maddegen-art/security/maddegen-art-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
---
