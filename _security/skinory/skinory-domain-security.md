---
api_specs:
- filename: skinory-inventories-api-openapi.yml
  format: yaml
  label: Skinory (submitted as g2push) Inventories API
  slug: skinory-inventories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/skinory/refs/heads/main/openapi/skinory-inventories-api-openapi.yml
- filename: skinory-inventory-api-openapi.yml
  format: yaml
  label: Skinory (submitted as g2push) Inventory API
  slug: skinory-inventory-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/skinory/refs/heads/main/openapi/skinory-inventory-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: skinory.io
  spf: true
hosts:
- cert_expires: Dec 26 11:20:54 2026 GMT
  host: skinory.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Skinory Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Skinory (submitted as g2push), probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC absent.'
provider_name: Skinory (submitted as g2push)
provider_slug: skinory
slug: skinory-domain-security
source_filename: skinory-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: skinory.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 26 11:20:54 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: skinory.io\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/skinory/refs/heads/main/security/skinory-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC
tags:
- Company
- Gaming
- Skins
- CS2
- CS:GO
- API
---
