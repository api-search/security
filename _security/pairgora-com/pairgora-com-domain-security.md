---
api_specs:
- filename: pairgora-com-openapi-generated.yml
  format: yaml
  label: Pairgora API
  slug: pairgora-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/pairgora-com/openapi/_ae-authored/pairgora-com-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: pairgora.com
  spf: false
hosts:
- cert_expires: Jan 14 14:17:33 2027 GMT
  host: pairgora.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Pairgora Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Pairgora, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=quarantine).'
provider_name: Pairgora
provider_slug: pairgora-com
slug: pairgora-com-domain-security
source_filename: pairgora-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: pairgora.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 14 14:17:33 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: pairgora.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/pairgora-com/security/pairgora-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Collaboration
- Artificial Intelligence
- MCP
- Human-Agent
- Platform
---
