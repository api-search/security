---
api_specs:
- filename: namailu-cz-acp-api-openapi.yml
  format: yaml
  label: namailu.cz Acp API
  slug: namailu-cz-acp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/namailu-cz/openapi/namailu-cz-acp-api-openapi.yml
- filename: namailu-cz-device-api-openapi.yml
  format: yaml
  label: namailu.cz Device API
  slug: namailu-cz-device-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/namailu-cz/openapi/namailu-cz-device-api-openapi.yml
- filename: namailu-cz-health-api-openapi.yml
  format: yaml
  label: namailu.cz Health API
  slug: namailu-cz-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/namailu-cz/openapi/namailu-cz-health-api-openapi.yml
- filename: namailu-cz-inboxes-api-openapi.yml
  format: yaml
  label: namailu.cz Inboxes API
  slug: namailu-cz-inboxes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/namailu-cz/openapi/namailu-cz-inboxes-api-openapi.yml
- filename: namailu-cz-key-rotation-api-openapi.yml
  format: yaml
  label: namailu.cz Key Rotation API
  slug: namailu-cz-key-rotation-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/namailu-cz/openapi/namailu-cz-key-rotation-api-openapi.yml
- filename: namailu-cz-messages-api-openapi.yml
  format: yaml
  label: namailu.cz Messages API
  slug: namailu-cz-messages-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/namailu-cz/openapi/namailu-cz-messages-api-openapi.yml
- filename: namailu-cz-metrics-api-openapi.yml
  format: yaml
  label: namailu.cz Metrics API
  slug: namailu-cz-metrics-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/namailu-cz/openapi/namailu-cz-metrics-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: namailu.cz
  spf: true
hosts:
- cert_expires: Jan  5 08:33:24 2027 GMT
  host: namailu.cz
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: namailu.cz Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for namailu.cz, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: namailu.cz
provider_slug: namailu-cz
slug: namailu-cz-domain-security
source_filename: namailu-cz-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: namailu.cz\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  5 08:33:24 2027 GMT\n  hsts: null\ndomains:\n- domain: namailu.cz\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/namailu-cz/security/namailu-cz-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Email Hosting
- AI Agents
- Webmail
- Organisations
---
