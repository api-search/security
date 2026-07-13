---
api_specs:
- filename: swagger.json
  format: json
  label: Coder REST API
  slug: rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/coder/coder/main/coderd/apidoc/swagger.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: coder.com
  spf: true
hosts:
- cert_expires: Aug 20 16:12:19 2026 GMT
  host: coder.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Coder Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Coder, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Coder
provider_slug: coder
slug: coder-domain-security
source_filename: coder-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: coder.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 20 16:12:19 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: coder.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/coder/refs/heads/main/security/coder-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Developer Tools
- Remote Development
- Cloud Development Environments
- AI Agents
- Infrastructure
- Workspaces
---
