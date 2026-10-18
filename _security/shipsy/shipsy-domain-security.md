---
api_specs:
- filename: shipsy-website-ai-api-openapi.yml
  format: yaml
  label: Shipsy Website AI API
  slug: shipsy-website-ai-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shipsy/refs/heads/main/openapi/shipsy-website-ai-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: shipsy.io
  spf: true
hosts:
- cert_expires: Dec 30 07:53:15 2026 GMT
  host: www.shipsy.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Shipsy Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Shipsy, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Shipsy
provider_slug: shipsy
slug: shipsy-domain-security
source_filename: shipsy-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.shipsy.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 30 07:53:15 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: shipsy.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/shipsy/refs/heads/main/security/shipsy-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Logistics
- Artificial Intelligence
- Transportation
- Warehouse
- Software-as-a-Service
- Company
---
