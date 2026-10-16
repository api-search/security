---
api_specs:
- filename: tado-openapi-generated.yml
  format: yaml
  label: tado API
  slug: tado-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tado/refs/heads/main/openapi/_ae-authored/tado-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: tado.com
  spf: true
hosts:
- cert_expires: Nov 19 03:33:43 2026 GMT
  host: www.tado.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Tado Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for tado, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: tado
provider_slug: tado
slug: tado-domain-security
source_filename: tado-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.tado.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 19 03:33:43 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: tado.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tado/refs/heads/main/security/tado-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- SmartHome
- Heating
- EnergySaving
- IoT
---
