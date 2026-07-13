---
api_specs:
- filename: tooljet-tooljet-external-api-openapi.yml
  format: yaml
  label: ToolJet External API
  slug: tooljet-external-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tooljet/refs/heads/main/openapi/tooljet-tooljet-external-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: tooljet.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: your-tooljet-instance.com
  spf: false
hosts:
- cert_expires: Sep 30 23:08:42 2026 GMT
  host: tooljet.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 30 23:08:42 2026 GMT
  host: docs.tooljet.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- host: your-tooljet-instance.com
  https: false
kind: domain-security
layout: security
method: probed
name: Tooljet Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ToolJet, probed live across 3 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: ToolJet
provider_slug: tooljet
slug: tooljet-domain-security
source_filename: tooljet-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: tooljet.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 23:08:42 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.tooljet.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 23:08:42 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: your-tooljet-instance.com\n  https: false\ndomains:\n- domain: tooljet.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: your-tooljet-instance.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tooljet/refs/heads/main/security/tooljet-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- low-code
- internal tools
- open-source
- application builder
- workflow automation
- no-code
- dashboards
- AI agents
---
