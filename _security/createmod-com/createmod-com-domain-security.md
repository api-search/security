---
api_specs:
- filename: createmod-com-analytics-api-openapi.yml
  format: yaml
  label: CreateMod.com Analytics API
  slug: createmod-com-analytics-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/createmod-com/openapi/createmod-com-analytics-api-openapi.yml
- filename: createmod-com-mod-integration-api-openapi.yml
  format: yaml
  label: CreateMod.com Mod Integration API
  slug: createmod-com-mod-integration-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/createmod-com/openapi/createmod-com-mod-integration-api-openapi.yml
- filename: createmod-com-schematics-api-openapi.yml
  format: yaml
  label: CreateMod.com Schematics API
  slug: createmod-com-schematics-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/createmod-com/openapi/createmod-com-schematics-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: createmod.com
  spf: true
hosts:
- cert_expires: Dec 12 15:11:58 2026 GMT
  host: createmod.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: CreateMod.com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CreateMod.com, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC absent.'
provider_name: CreateMod.com
provider_slug: createmod-com
slug: createmod-com-domain-security
source_filename: createmod-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: createmod.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 12 15:11:58 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: createmod.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/createmod-com/security/createmod-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC
tags:
- Company
- Minecraft
- Gaming
- Schematics
- Create Mod
- Community
- User Generated Content
- REST API
---
