---
api_specs:
- filename: anchorbrowser-openapi.yml
  format: yaml
  label: Anchor Browser API
  slug: anchor-browser-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anchorbrowser/refs/heads/main/openapi/anchorbrowser-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: anchorbrowser.io
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: browsermcp.com
  spf: true
hosts:
- cert_expires: Sep 12 11:55:38 2026 GMT
  host: anchorbrowser.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 13 21:07:48 2026 GMT
  host: docs.anchorbrowser.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 14 00:36:46 2026 GMT
  host: browsermcp.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Anchorbrowser Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Anchor Browser, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Anchor Browser
provider_slug: anchorbrowser
slug: anchorbrowser-domain-security
source_filename: anchorbrowser-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: anchorbrowser.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 12 11:55:38 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.anchorbrowser.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 13 21:07:48 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: browsermcp.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 14 00:36:46 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: anchorbrowser.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: browsermcp.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/anchorbrowser/refs/heads/main/security/anchorbrowser-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Browser Infrastructure
- AI Agents
- Cloud Browser
- Browser Automation
- Sandbox
- Stealth Browser
- MCP
---
