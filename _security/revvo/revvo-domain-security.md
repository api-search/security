---
api_specs:
- filename: revvo-api-openapi-original.yml
  format: yaml
  label: Revvo API
  slug: revvo-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/revvo/refs/heads/main/openapi/revvo-api-openapi-original.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: revvo.ai
  spf: true
hosts:
- cert_expires: Oct  3 23:08:27 2026 GMT
  host: revvo.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Revvo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Revvo, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Revvo
provider_slug: revvo
slug: revvo-domain-security
source_filename: revvo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: revvo.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 23:08:27 2026 GMT\n  hsts: false\ndomains:\n- domain: revvo.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/revvo/refs/heads/main/security/revvo-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Fleet Management
- Transportation
- Tire Management
- TPMS
- Telematics
- IoT
- Logistics
- API
---
