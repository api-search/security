---
api_specs:
- filename: atomicwork-public-api-openapi.yaml
  format: yaml
  label: Atomicwork Public API
  slug: atomicwork-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/atomicwork/refs/heads/main/openapi/atomicwork-public-api-openapi.yaml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: atomicwork.com
  spf: true
hosts:
- cert_expires: Aug 27 20:16:15 2026 GMT
  host: www.atomicwork.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 13 03:51:46 2026 GMT
  host: developers.atomicwork.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Atomicwork Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Atomicwork, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Atomicwork
provider_slug: atomicwork
slug: atomicwork-domain-security
source_filename: atomicwork-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.atomicwork.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 27 20:16:15 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developers.atomicwork.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 03:51:46 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: atomicwork.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/atomicwork/refs/heads/main/security/atomicwork-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Service Management
- ITSM
- ESM
- IT Service Desk
- Identity Governance
- Asset Management
- AI Agents
- MCP
- Enterprise
---
