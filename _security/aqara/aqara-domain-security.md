---
api_specs:
- filename: aqara-automation-api-openapi.yml
  format: yaml
  label: Aqara Automation API
  slug: aqara-automation-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aqara/openapi/aqara-automation-api-openapi.yml
- filename: aqara-device-api-openapi.yml
  format: yaml
  label: Aqara Device API
  slug: aqara-device-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aqara/openapi/aqara-device-api-openapi.yml
- filename: aqara-gateway-api-openapi.yml
  format: yaml
  label: Aqara Gateway API
  slug: aqara-gateway-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aqara/openapi/aqara-gateway-api-openapi.yml
- filename: aqara-space-api-openapi.yml
  format: yaml
  label: Aqara Space API
  slug: aqara-space-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aqara/openapi/aqara-space-api-openapi.yml
- filename: aqara-studio-api-openapi.yml
  format: yaml
  label: Aqara Studio API
  slug: aqara-studio-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aqara/openapi/aqara-studio-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: aqara.com
  spf: true
hosts:
- cert_expires: Jan  7 06:43:16 2027 GMT
  host: aqara.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Aqara Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Aqara, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Aqara
provider_slug: aqara
slug: aqara-domain-security
source_filename: aqara-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: aqara.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  7 06:43:16 2027 GMT\n  hsts: false\ndomains:\n- domain: aqara.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/aqara/security/aqara-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Smart Home
- IoT
- Consumer Electronics
- Home Automation
- Security
---
