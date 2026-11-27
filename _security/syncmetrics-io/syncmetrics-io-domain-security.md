---
api_specs:
- filename: syncmetrics-io-api-openapi.json
  format: json
  label: FastAPI API
  slug: fastapi-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/syncmetrics-io/openapi/_original/syncmetrics-io-api-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dns_aid:
    checked: '2026-11-25'
    published: false
  dnssec: false
  domain: syncmetrics.io
  spf: true
hosts:
- cert_expires: Feb  4 13:06:09 2027 GMT
  host: syncmetrics.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: SyncMetrics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SyncMetrics, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: SyncMetrics
provider_slug: syncmetrics-io
slug: syncmetrics-io-domain-security
source_filename: syncmetrics-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: syncmetrics.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  4 13:06:09 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: syncmetrics.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n  dns_aid:\n    checked: '2026-11-25'\n    published: false\n"
source_yaml_url: https://artifacts.apis.io/syncmetrics-io/security/syncmetrics-io-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Marketing
- Analytics
- AI
- Advertising
- DataIntegration
---
