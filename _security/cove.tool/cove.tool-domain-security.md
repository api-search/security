---
api_specs:
- filename: cove.tool-rest-api-v2-openapi.yml
  format: yaml
  label: cove.tool REST API v2
  slug: rest-api-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cove.tool/refs/heads/main/openapi/cove.tool-rest-api-v2-openapi.yml
- filename: cove.tool-api-v1-openapi.yml
  format: yaml
  label: cove.tool API v1
  slug: api-v1
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cove.tool/refs/heads/main/openapi/cove.tool-api-v1-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: cove.inc
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: covetool.com
  spf: true
hosts:
- cert_expires: Nov  6 23:03:07 2026 GMT
  host: cove.inc
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 23 12:34:42 2026 GMT
  host: developers.covetool.com
  hsts: false
  https: true
  tls_version: TLSv1.2
- cert_expires: Sep  3 23:59:59 2026 GMT
  host: app.covetool.com
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Cove.Tool Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cove.Tool, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Cove.Tool
provider_slug: cove.tool
slug: cove.tool-domain-security
source_filename: cove.tool-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cove.inc\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  6 23:03:07 2026 GMT\n  hsts: false\n- host: developers.covetool.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 23 12:34:42 2026 GMT\n  hsts: false\n- host: app.covetool.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep  3 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: cove.inc\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: covetool.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cove.tool/refs/heads/main/security/cove.tool-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Building Performance
- Energy Modeling
- Daylight Analysis
- Sustainability
- Architecture
- AEC
- Simulation
- Embodied Carbon
- Building Design
---
