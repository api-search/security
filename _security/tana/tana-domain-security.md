---
api_specs:
- filename: tana-input-api-openapi.yml
  format: yaml
  label: Tana Input API
  slug: tana-input-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tana/refs/heads/main/openapi/tana-input-api-openapi.yml
- filename: tana-docs-api-openapi.yml
  format: yaml
  label: Tana Documentation API
  slug: tana-documentation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tana/refs/heads/main/openapi/tana-docs-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: tana.inc
  spf: true
hosts:
- cert_expires: Sep 14 02:17:58 2026 GMT
  host: tana.inc
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Tana Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Tana, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Tana
provider_slug: tana
slug: tana-domain-security
source_filename: tana-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: tana.inc\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 02:17:58 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: tana.inc\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tana/refs/heads/main/security/tana-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Note Taking
- Knowledge Management
- Productivity
- Artificial Intelligence
- Meetings
- Agents
- Collaboration
- Outliner
---
