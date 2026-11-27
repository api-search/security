---
api_specs:
- filename: grip-fyi-compare-api-openapi.yml
  format: yaml
  label: GRIP Compare API
  slug: grip-fyi-compare-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/grip-fyi/openapi/grip-fyi-compare-api-openapi.yml
- filename: grip-fyi-embed-api-openapi.yml
  format: yaml
  label: GRIP Embed API
  slug: grip-fyi-embed-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/grip-fyi/openapi/grip-fyi-embed-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: grip.fyi
  spf: false
hosts:
- cert_expires: Dec 30 18:51:10 2026 GMT
  host: grip.fyi
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: GRIP Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for GRIP, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: GRIP
provider_slug: grip-fyi
slug: grip-fyi-domain-security
source_filename: grip-fyi-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-10'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: grip.fyi\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 30 18:51:10 2026 GMT\n  hsts: false\ndomains:\n- domain: grip.fyi\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/grip-fyi/security/grip-fyi-domain-security.yml
summary_line: TLSv1.3
tags:
- Discovery
- Invocation
- Capabilities
- Machine
- Blockchain
- Robotics
---
