---
api_specs:
- filename: agenticrail-nz-enforcement-api-openapi.yml
  format: yaml
  label: AgenticRail Enforcement API
  slug: agenticrail-nz-enforcement-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agenticrail-nz/openapi/agenticrail-nz-enforcement-api-openapi.yml
- filename: agenticrail-nz-evidence-api-openapi.yml
  format: yaml
  label: AgenticRail Evidence API
  slug: agenticrail-nz-evidence-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agenticrail-nz/openapi/agenticrail-nz-evidence-api-openapi.yml
- filename: agenticrail-nz-operational-api-openapi.yml
  format: yaml
  label: AgenticRail Operational API
  slug: agenticrail-nz-operational-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agenticrail-nz/openapi/agenticrail-nz-operational-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: agenticrail.nz
  spf: true
hosts:
- cert_expires: Jan  8 11:16:46 2027 GMT
  host: agenticrail.nz
  hsts: true
  hsts_max_age: 0
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: AgenticRail Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AgenticRail, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: AgenticRail
provider_slug: agenticrail-nz
slug: agenticrail-nz-domain-security
source_filename: agenticrail-nz-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: agenticrail.nz\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  8 11:16:46 2027 GMT\n  hsts: true\n  hsts_max_age: 0\ndomains:\n- domain: agenticrail.nz\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/agenticrail-nz/security/agenticrail-nz-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Artificial Intelligence
- Automation
- Sequence Enforcement
- Cryptographic Receipts
- Compliance
---
