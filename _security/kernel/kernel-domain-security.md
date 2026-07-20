---
api_specs:
- filename: kernel-openapi-original.yml
  format: yaml
  label: Kernel API
  slug: kernel-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kernel/refs/heads/main/openapi/kernel-openapi-original.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: onkernel.com
  spf: true
hosts:
- cert_expires: Dec 26 23:59:59 2026 GMT
  host: api.onkernel.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Kernel Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Kernel, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Kernel
provider_slug: kernel
slug: kernel-domain-security
source_filename: kernel-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: api.onkernel.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 26 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: onkernel.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kernel/refs/heads/main/security/kernel-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Browser Automation
- Web Agents
- Browser Infrastructure
- AI Agents
- Playwright
- Cloud Browsers
- Computer Use
- MCP
- Managed Auth
---
