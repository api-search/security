---
api_specs:
- filename: aiogeoprotocol-com-audit-api-openapi.yml
  format: yaml
  label: AIO.GEO Protocol Audit API
  slug: aiogeoprotocol-com-audit-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aiogeoprotocol-com/openapi/aiogeoprotocol-com-audit-api-openapi.yml
- filename: aiogeoprotocol-com-brief-api-openapi.yml
  format: yaml
  label: AIO.GEO Protocol Brief API
  slug: aiogeoprotocol-com-brief-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aiogeoprotocol-com/openapi/aiogeoprotocol-com-brief-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: aiogeoprotocol.com
  spf: false
hosts:
- cert_expires: Jan  9 12:01:44 2027 GMT
  host: aiogeoprotocol.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: AIO.GEO Protocol Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AIO.GEO Protocol, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF absent, DMARC present (p=quarantine).'
provider_name: AIO.GEO Protocol
provider_slug: aiogeoprotocol-com
slug: aiogeoprotocol-com-domain-security
source_filename: aiogeoprotocol-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: aiogeoprotocol.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  9 12:01:44 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: aiogeoprotocol.com\n  dnssec: true\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/aiogeoprotocol-com/security/aiogeoprotocol-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Artificial Intelligence
- Search
- Audit
- Measurements
- CLI
---
