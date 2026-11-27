---
api_specs:
- filename: outage-me-contribute-api-key-opt-in-api-openapi.yml
  format: yaml
  label: outage.me Contribute — API key, opt-in API
  slug: outage-me-contribute-api-key-opt-in-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/outage-me/openapi/outage-me-contribute-api-key-opt-in-api-openapi.yml
- filename: outage-me-layer-1-open-no-key-api-openapi.yml
  format: yaml
  label: outage.me Layer 1 — open, no key API
  slug: outage-me-layer-1-open-no-key-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/outage-me/openapi/outage-me-layer-1-open-no-key-api-openapi.yml
- filename: outage-me-layer-2-api-key-api-openapi.yml
  format: yaml
  label: outage.me Layer 2 — API key API
  slug: outage-me-layer-2-api-key-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/outage-me/openapi/outage-me-layer-2-api-key-api-openapi.yml
- filename: outage-me-webhooks-pro-api-key-api-openapi.yml
  format: yaml
  label: outage.me Webhooks — Pro API key API
  slug: outage-me-webhooks-pro-api-key-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/outage-me/openapi/outage-me-webhooks-pro-api-key-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: outage.me
  spf: true
hosts:
- cert_expires: Apr 27 23:59:59 2027 GMT
  host: outage.me
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: outage.me Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for outage.me, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: outage.me
provider_slug: outage-me
slug: outage-me-domain-security
source_filename: outage-me-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: outage.me\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Apr 27 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: outage.me\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/outage-me/security/outage-me-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Status
- Monitoring
- Real-Time
- Cloud
---
